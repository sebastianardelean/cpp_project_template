# Generic test that uses conan libs

set(src 
        main.cpp 
    )
set(inc 
    )
add_executable(intro ${src} ${inc})
target_link_libraries(
  intro
          CONAN_PKG::fmt
          CONAN_PKG::spdlog)
