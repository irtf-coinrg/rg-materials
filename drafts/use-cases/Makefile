draftname="draft-irtf-coinrg-use-cases"
all:
ifdef v
	kramdown-rfc version-$(v)/$(draftname)-$(v).mkd > version-$(v)/$(draftname)-$(v).xml
	sed -e "s/symRefs=\"true\"/symRefs=\"true\" tocDepth=\"2\"/" version-$(v)/$(draftname)-$(v).xml > tmp.xml
	sed -e "s/ü/ue/g" tmp.xml > tmp2.xml
	sed -e "s/Ruth/Rueth/g" tmp2.xml > tmp.xml
	sed -e "s/”/\"/g" tmp.xml > tmp2.xml
	sed -e "s/“/\"/g" tmp2.xml > tmp.xml
	sed -e "s/é/e/g" tmp.xml > tmp2.xml
	sed -e "s/ó/o/g" tmp2.xml > tmp.xml
	mv tmp.xml version-$(v)/$(draftname)-$(v).xml
	xml2rfc version-$(v)/$(draftname)-$(v).xml
	rm tmp2.xml
	grep --color='auto' -P -n "[\x80-\xFF]" version-$(v)/$(draftname)-$(v).txt
else
	@echo 'State version using v='
endif