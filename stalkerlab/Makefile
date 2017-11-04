# $Id$

DOCUMENTS=	privacy.pdf
FILES=		privacy.tex aims.tex literature.tex literature.bib
CATEGORY=	security/labs
PACKAGE=	privacy-src
PACKAGE_FILES=	${FILES} Makefile
PUB_FILES=	${DOCUMENTS} ${PACKAGE}.tar.gz

privacy.pdf: ${FILES}

#export no

Makefile.export: Makefile
PACKAGE_FILES=	${FILES:.tex=.exporttex} Makefile.export

literature.bib: ../../infosak.bib
	${CP} $^ $@

clean:
	${RM} literature.bib

#endexport

### INCLUDES ###

INCLUDES= 	depend.mk miun.course.mk miun.package.mk

define inc
ifeq ($(findstring $(1),${MAKEFILE_LIST}),)
$(1):
	wget https://raw.githubusercontent.com/dbosk/makefiles/master/$(1)
include $(1)
endif
endef
$(foreach i,${INCLUDES},$(eval $(call inc,$i)))
