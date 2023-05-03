add_executable(template_mipt_tests variant_tests.cpp)

target_link_libraries(template_mipt_tests ${LIB_TARGET} GTest::gtest_main)

include(GoogleTest)
gtest_discover_tests(template_mipt_tests)

set_target_properties(
        template_mipt_tests
        PROPERTIES
        CXX_STANDARD 20
        CXX_STANDARD_REQUIRED ON)