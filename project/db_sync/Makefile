
ifndef SUPPORTCMDS
SUPPORTCMDS:= all objs clean cleanall rebuild
endif

MAKEFILENAME:= Makefile_src

$(SUPPORTCMDS):
	for filename in $(MAKEFILENAME); do \
		echo "Making " $$filename $@ ; \
		(make $@ -f $$filename || exit "$$?"); \
	done;
