# Copyright 2022 The OpenXLA Authors
#
# Licensed under the Apache License v2.0 with LLVM Exceptions.
# See https://llvm.org/LICENSE.txt for license information.
# SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception

iree_lit_test_suite(
  NAME
    lit
  SRCS
    "example.mlir"
  TOOLS
    FileCheck
    iree-compile
    openxla-runner
  LABELS
    "hostonly"
)
