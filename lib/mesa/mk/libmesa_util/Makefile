#	$OpenBSD: Makefile,v 1.1 2020/08/26 06:02:40 jsg Exp $

LIB=	mesa_util

NOPROFILE=

SRCS=	anon_file.c \
	bitscan.c \
	blob.c \
	build_id.c \
	crc32.c \
	dag.c \
	debug.c \
	disk_cache.c \
	double.c \
	fast_idiv_by_const.c \
	half_float.c \
	hash_table.c \
	mesa-sha1.c \
	os_file.c \
	os_misc.c \
	os_socket.c \
	os_time.c \
	ralloc.c \
	rand_xor.c \
	rb_tree.c \
	register_allocate.c \
	rgtc.c \
	set.c \
	sha1.c \
	slab.c \
	softfloat.c \
	sparse_array.c \
	string_buffer.c \
	strtod.c \
	u_atomic.c \
	u_cpu_detect.c \
	u_debug.c \
	u_debug_memory.c \
	u_math.c \
	u_mm.c \
	u_process.c \
	u_queue.c \
	u_vector.c \
	vma.c

SRCS+=	format_srgb.c

.include "../Makefile.inc"

CFLAGS+=	${C_VIS_ARGS}
CPPFLAGS+=	-I${MESA_SRC}/src/util \
		-I${MESA_SRC}/src/mesa \
		-I${MESA_SRC}/src/gallium/include \
		-I${MESA_SRC}/src/gallium/auxiliary

install:

obj: _xenocara_obj

.include <bsd.lib.mk>
.include <bsd.xorg.mk>

.PATH: ${MESA_SRC}/src/util
.PATH: ${MESA_SRC}/src/util/sha1
.PATH: ${MESA_SRC}/generated/src/util
