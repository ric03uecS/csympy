project(test_eval)

if (HAVE_CSYMPY_ARB)
    add_executable(test_eval_arb test_eval_arb.cpp)
    target_link_libraries(test_eval_arb csympy)
    add_test(test_eval_arb ${PROJECT_BINARY_DIR}/test_eval_arb)
endif()
