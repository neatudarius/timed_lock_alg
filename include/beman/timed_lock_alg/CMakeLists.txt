# SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception

target_sources(
    beman.timed_lock_alg
    PUBLIC FILE_SET HEADERS FILES timed_lock_alg.hpp mutex.hpp
)
