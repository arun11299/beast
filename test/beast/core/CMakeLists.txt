#
# Copyright (c) 2016-2017 Vinnie Falco (vinnie dot falco at gmail dot com)
#
# Distributed under the Boost Software License, Version 1.0. (See accompanying
# file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt)
#
# Official repository: https://github.com/boostorg/beast
#

GroupSources(extras/boost/beast extras)
GroupSources(include/boost/beast beast)
GroupSources(test/beast/core "/")

add_executable (tests-beast-core
    ${BOOST_BEAST_INCLUDES}
    ${EXTRAS_INCLUDES}
    ${TEST_MAIN}
    Jamfile
    buffer_test.hpp
    file_test.hpp
    async_result.cpp
    bind_handler.cpp
    buffer_cat.cpp
    buffer_prefix.cpp
    buffered_read_stream.cpp
    buffers_adapter.cpp
    clamp.cpp
    consuming_buffers.cpp
    drain_buffer.cpp
    error.cpp
    file.cpp
    file_posix.cpp
    file_stdio.cpp
    file_win32.cpp
    flat_buffer.cpp
    flat_static_buffer.cpp
    handler_alloc.cpp
    handler_ptr.cpp
    multi_buffer.cpp
    ostream.cpp
    read_size.cpp
    span.cpp
    static_string.cpp
    string.cpp
    static_buffer.cpp
    string_param.cpp
    type_traits.cpp
    base64.cpp
    empty_base_optimization.cpp
    sha1.cpp
    detail/variant.cpp
    detail/varint.cpp
)
