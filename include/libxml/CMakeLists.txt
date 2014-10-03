SET(WITH_TRIO
  0)

SET(WITH_THREADS
  1)

SET(WITH_THREAD_ALLOC 1)

SET(WITH_TREE 1)
SET(WITH_OUTPUT 1)
SET(WITH_PUSH 1)
SET(WITH_READER 1)
SET(WITH_PATTERN 1)
SET(WITH_WRITER 1)
SET(WITH_SAX1 1)
SET(WITH_FTP 0)
SET(WITH_HTTP 0)
SET(WITH_VALID 1)
SET(WITH_HTML 1)
SET(WITH_LEGACY 0)
SET(WITH_C14N 1)
SET(WITH_CATALOG 1)
SET(WITH_DOCB 0)
SET(WITH_XPATH 1)
SET(WITH_XPTR 1)
SET(WITH_XINCLUDE 1)
SET(WITH_ICONV 0)
SET(WITH_ICU 0)
SET(WITH_ISO8859X 1)
SET(WITH_DEBUG 1)
SET(WITH_MEM_DEBUG 1)
SET(WITH_RUN_DEBUG 1)
SET(WITH_REGEXPS 1)
SET(WITH_SCHEMAS 1)
SET(WITH_SCHEMATRON 1)
SET(WITH_MODULES 1)
SET(WITH_ZLIB 1)
SET(WITH_LZMA 1)
SET(LIBXML_VERSION_NUMBER 20700)

configure_file(${CMAKE_CURRENT_SOURCE_DIR}/xmlversion.h.in ${CMAKE_CURRENT_BINARY_DIR}/xmlversion.h)

configure_file(${CMAKE_CURRENT_SOURCE_DIR}/xmlwin32version.h.in ${CMAKE_CURRENT_BINARY_DIR}/xmlwin32version.h)


########### install files ###############

install(FILES  DESTINATION include/libxml2/libxml)



#original Makefile.am contents follow:

### Process this file with automake to produce Makefile.in
#
#xmlincdir = $(includedir)/libxml2/libxml
#
#xmlinc_HEADERS = \
#		SAX.h \
#		entities.h \
#		encoding.h \
#		parser.h \
#		parserInternals.h \
#		xmlerror.h \
#		HTMLparser.h \
#		HTMLtree.h \
#		debugXML.h \
#		tree.h \
#		list.h \
#		hash.h \
#		xpath.h \
#		xpathInternals.h \
#		xpointer.h \
#		xinclude.h \
#		xmlIO.h \
#		xmlmemory.h \
#		nanohttp.h \
#		nanoftp.h \
#		uri.h \
#		valid.h \
#		xlink.h \
#		xmlversion.h \
#		DOCBparser.h \
#		catalog.h \
#		threads.h \
#		globals.h \
#		c14n.h \
#		xmlautomata.h \
#		xmlregexp.h \
#		xmlmodule.h \
#		xmlschemas.h \
#		schemasInternals.h \
#		xmlschemastypes.h \
#		xmlstring.h \
#		xmlunicode.h \
#		xmlreader.h \
#		relaxng.h \
#		dict.h \
#		SAX2.h \
#		xmlexports.h \
#		xmlwriter.h \
#		chvalid.h \
#		pattern.h \
#		xmlsave.h \
#		schematron.h
#
#EXTRA_DIST = xmlversion.h.in
