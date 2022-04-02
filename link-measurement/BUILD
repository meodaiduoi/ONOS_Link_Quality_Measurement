COMPILE_DEPS = CORE_DEPS + JACKSON + METRICS + CLI + REST + [
    "//core/common:onos-core-common",
    #    "//drivers/default:onos-drivers-default",
]

osgi_jar_with_tests(
    api_description = "BigMao Radio Station REST API v1.0, for link quality measurement",
    api_package = "org.onosproject.linkmeasurement.rest",
    api_title = "BigMao Radio Station REST API v1.0",
    api_version = "/onos/v1/linkmeasurement",
    karaf_command_packages = ["org.onosproject.linkmeasurement.cli"],
    web_context = "/onos/linkmeasurement",
    deps = COMPILE_DEPS,
)

REQUIRE_APPS = [
    #    "org.onosproject.proxyarp",
]

onos_app(
    app_name = "org.onosproject.linkmeasurement",
    category = "Monitoring",
    description = "Mao Link Quality Measurement",
    required_apps = REQUIRE_APPS,
    title = "Mao Link Quality Measurement",
    url = "https://www.maojianwei.com",
)