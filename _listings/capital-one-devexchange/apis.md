---
name: Capital One DevExchange
x-slug: capital-one-devexchange
description: What unites us all is a desire to create better end customer experiences.
  Were building a full suite of tools and technology that make essential things in
  peoples everyday life &ndash; money, finances, identity &ndash; simpler for you.
  Now is the time to join our beta program, and help us shape the future.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Transfers
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/apis.md
specificationVersion: "0.14"
apis:
- name: Capital One DevExchange Get all transfers
  x-api-slug: capital-one-devexchange
  description: Returns the transfers that you are involved in.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/transfers
  tags: Banks,Accounts, , Transfers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/accountsidtransfers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/accountsidtransfers-get-openapi.md
- name: Capital One DevExchange Create a transfer
  x-api-slug: capital-one-devexchange
  description: Creates a transfer where the account with the ID specified is the payer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////accounts/{id}/transfers
  tags: Banks,Accounts, , Transfers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/accountsidtransfers-post-openapi.md
- name: Capital One DevExchange Get transfer by id
  x-api-slug: capital-one-devexchange
  description: Returns the transfer with the specific id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////transfers/{transferId}
  tags: Banks,Transfers, Transfer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/transferstransferid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/transferstransferid-get-openapi.md
- name: Capital One DevExchange Update a specific existing transfer
  x-api-slug: capital-one-devexchange
  description: Updates the specific transfer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////transfers/{transferId}
  tags: Banks,Transfers, Transfer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/transferstransferid-put-openapi.md
- name: Capital One DevExchange Delete a specific existing transfer
  x-api-slug: capital-one-devexchange
  description: Deletes the specific transfer
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com////transfers/{transferId}
  tags: Banks,Transfers, Transfer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/transferstransferid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/transferstransferid-delete-openapi.md
- name: Capital One DevExchange
  x-api-slug: capital-one-devexchange
  description: What unites us all is a desire to create better end customer experiences.
    Were building a full suite of tools and technology that make essential things
    in peoples everyday life &ndash; money, finances, identity &ndash; simpler for
    you. Now is the time to join our beta program, and help us shape the future.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/capitalone-devexchange.png
  humanURL: http://capitalone.com
  baseURL: https://api.reimaginebanking.com//
  tags: Transfers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/capital-one-devexchange/openapi.md
x-common:
- type: x-authentication
  url: https://developer.capitalone.com/platform-documentation/authorization-with-oauth-20/
- type: x-blog
  url: https://developer.capitalone.com/blogs/
- type: x-developer
  url: https://developer.capitalone.com/
- type: x-documentation
  url: https://developer.capitalone.com/platform-documentation/
- type: x-errors
  url: https://developer.capitalone.com/platform-documentation/errors/
- type: x-getting-started
  url: https://developer.capitalone.com/platform-documentation/getting-started/
- type: x-github
  url: https://github.com/capitalone
- type: x-website
  url: http://capitalone.com
- type: x-open-source
  url: https://developer.capitalone.com/open-source/
- type: x-sandbox
  url: https://developer.capitalone.com/platform-documentation/using-the-sandbox/
- type: x-login
  url: https://developer.capitalone.com/sign-in/
- type: x-selfservice-registration
  url: https://developer.capitalone.com/sign-up
- type: x-support
  url: https://developer.capitalone.com/support/
- type: x-privacy-policy
  url: https://www.capitalone.com/identity-protection/privacy/statement
- type: x-terms-of-service
  url: https://developer.capitalone.com/single/terms-and-conditions/
- type: x-twitter
  url: https://twitter.com/CapitalOneDevEx
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---