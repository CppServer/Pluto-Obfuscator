add_llvm_component_library(LLVMObfuscation
  HelloWorld.cpp
  SplitBasicBlock.cpp
  CryptoUtils.cpp
  Utils.cpp
  Flattening.cpp
  BogusControlFlow.cpp
  Substitution.cpp
  GlobalsEncryption.cpp
  VariableSubstitution.cpp
  RandomControlFlow.cpp
  TrapAngr.cpp
  MBAObfuscation.cpp
  MBAUtils.cpp

  DEPENDS
  intrinsics_gen
  
  LINK_LIBS
  z3

  LINK_COMPONENTS
  Core
  Support
  Analysis
  TransformUtils
)
  