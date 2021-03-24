all:
ifdef v
	kramdown-rfc2629 version-$(v)/draft-irtf-coinrg-use-cases-$(v).mkd > version-$(v)/draft-irtf-coinrg-use-cases-$(v).xml
	xml2rfc version-$(v)/draft-irtf-coinrg-use-cases-$(v).xml
	rm version-$(v)/draft-irtf-coinrg-use-cases-$(v).xml
else
	@echo 'State version using v='
endif