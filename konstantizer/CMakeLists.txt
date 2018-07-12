set(LLVM_LINK_COMPONENTS support)

add_clang_executable(konstantizer
  Konstantizer.cpp
  )
target_link_libraries(konstantizer
  PRIVATE
  clangTooling
  clangBasic
  clangASTMatchers
  )
