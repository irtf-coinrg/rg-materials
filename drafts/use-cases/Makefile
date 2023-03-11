draftname="draft-irtf-coinrg-use-cases"
all:
ifdef v
	kramdown-rfc version-$(v)/$(draftname)-$(v).mkd > version-$(v)/$(draftname)-$(v).xml
	sed -e "s/symRefs=\"true\"/symRefs=\"true\" tocDepth=\"2\"/" version-$(v)/$(draftname)-$(v).xml > tmp.xml
	sed -e "s/Rüth/Rueth/g" tmp.xml > tmp2.xml
	mv tmp2.xml version-$(v)/$(draftname)-$(v).xml
	xml2rfc version-$(v)/$(draftname)-$(v).xml
	rm tmp.xml
else
	@echo 'State version using v='
endif