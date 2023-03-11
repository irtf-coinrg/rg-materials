draftname="draft-irtf-coinrg-use-case-analysis"
all:
ifdef v
	kramdown-rfc version-$(v)/$(draftname)-$(v).mkd > version-$(v)/$(draftname)-$(v).xml
	xml2rfc version-$(v)/$(draftname)-$(v).xml
	#rm version-$(v)/$(draftname)-$(v).xml
else
	@echo 'State version using v='
endif

fromxml:
ifdef v
	xml2rfc version-$(v)/$(draftname)-$(v).xml
	#rm version-$(v)/$(draftname)-$(v).xml
else
	@echo 'State version using v='
endif