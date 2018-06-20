---
name: Stripe
x-slug: stripe
description: Online payment processing for internet businesses. Stripe is a suite
  of payment APIs that powers commerce for online businesses of all sizes, including
  fraud prevention, and subscription management. Use Stripe???s payment platform to
  accept and process p...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
x-kinRank: "10"
x-alexaRank: "1793"
tags: Transfers
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/apis.md
specificationVersion: "0.14"
apis:
- name: Stripe Get Transfers
  x-api-slug: stripe
  description: Returns a list of existing transfers sent to connected accounts. The
    transfers are returned in sorted order, with the most recently created transfers
    appearing first.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers
  tags: Transfers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfers-get-openapi.md
- name: Stripe Add Transfers
  x-api-slug: stripe
  description: Post Transfers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers
  tags: Transfers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfers-post-openapi.md
- name: Stripe Get Transfers  Reversals
  x-api-slug: stripe
  description: You can see a list of the reversals belonging to a specific transfer.
    Note that the 10 most recent reversals are always available by default on the
    transfer object. If you need more than those 10, you can use this API method and
    the limit and starting_after parameters to page through additional reversals.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{id}/reversals
  tags: Transfers, , Reversals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfersidreversals-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfersidreversals-get-openapi.md
- name: Stripe Add Transfers  Reversals
  x-api-slug: stripe
  description: Post Transfers, , Reversals
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{id}/reversals
  tags: Transfers, , Reversals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transfersidreversals-post-openapi.md
- name: Stripe Get Transfers Transfer
  x-api-slug: stripe
  description: Retrieves the details of an existing transfer. Supply the unique transfer
    ID from either a transfer creation request or the transfer list, and Stripe will
    return the corresponding transfer information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{transfer}
  tags: Transfers, Transfer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransfer-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransfer-get-openapi.md
- name: Stripe Add Transfers Transfer
  x-api-slug: stripe
  description: Post Transfers, Transfer
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{transfer}
  tags: Transfers, Transfer
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransfer-post-openapi.md
- name: Stripe Get Transfers Transfer Reversals
  x-api-slug: stripe
  description: By default, you can see the 10 most recent reversals stored directly
    on the transfer object, but you can also retrieve details about a specific reversal
    stored on the transfer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{transfer}/reversals/{id}
  tags: Transfers, Transfer, Reversals
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransferreversalsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransferreversalsid-get-openapi.md
- name: Stripe Add Transfers Transfer Reversals
  x-api-slug: stripe
  description: Updates the specified reversal by setting the values of the parameters
    passed. Any parameters not provided will be left unchanged.This request only accepts
    metadata and description as arguments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1///transfers/{transfer}/reversals/{id}
  tags: Transfers, Transfer, Reversals
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/transferstransferreversalsid-post-openapi.md
- name: Stripe
  x-api-slug: stripe
  description: Web and mobile payments, built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/254-stripe.jpg
  humanURL: https://stripe.com/
  baseURL: https://api.stripe.com/v1/
  tags: Transfers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/transfers/master/_listings/stripe/openapi.md
x-common:
- type: x-base
  url: https://api.stripe.com/
- type: x-blog
  url: https://stripe.com/blog
- type: x-blog-rss
  url: https://stripe.com/blog/feed.rss
- type: x-change-log
  url: https://stripe.com/docs/upgrades
- type: x-crunchbase
  url: http://www.crunchbase.com/company/stripe
- type: x-crunchbase
  url: https://crunchbase.com/organization/stripe
- type: x-email
  url: info@stripe.com
- type: x-email
  url: privacy@stripe.com
- type: x-email
  url: atlas@stripe.com
- type: x-email
  url: notices@stripe.com
- type: x-email
  url: jane.diaz@stripe.com
- type: x-email
  url: nonprofit@stripe.com
- type: x-email
  url: support@stripe.com
- type: x-github
  url: https://github.com/stripe
- type: x-pricing
  url: https://stripe.com/us/pricing
- type: x-twitter
  url: https://twitter.com/stripe
- type: x-website
  url: https://stripe.com/
- type: x-website
  url: http://stripe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---