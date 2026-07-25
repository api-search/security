---
api_specs:
- filename: amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace CancelChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-cancelchangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-cancelchangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DeleteResourcePolicy#resourceArn API
  slug: amazon-marketplace-deleteresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-deleteresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeChangeSet#catalog&changeSetId API
  slug: amazon-marketplace-describechangeset-catalog-changesetid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describechangeset-catalog-changesetid-api-openapi.yml
- filename: amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
  format: yaml
  label: Amazon Marketplace DescribeEntity#catalog&entityId API
  slug: amazon-marketplace-describeentity-catalog-entityid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-describeentity-catalog-entityid-api-openapi.yml
- filename: amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon Marketplace GetResourcePolicy#resourceArn API
  slug: amazon-marketplace-getresourcepolicy-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-getresourcepolicy-resourcearn-api-openapi.yml
- filename: amazon-marketplace-listchangesets-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListChangeSets API
  slug: amazon-marketplace-listchangesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listchangesets-api-openapi.yml
- filename: amazon-marketplace-listentities-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListEntities API
  slug: amazon-marketplace-listentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listentities-api-openapi.yml
- filename: amazon-marketplace-listtagsforresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace ListTagsForResource API
  slug: amazon-marketplace-listtagsforresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-listtagsforresource-api-openapi.yml
- filename: amazon-marketplace-putresourcepolicy-api-openapi.yml
  format: yaml
  label: Amazon Marketplace PutResourcePolicy API
  slug: amazon-marketplace-putresourcepolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-putresourcepolicy-api-openapi.yml
- filename: amazon-marketplace-startchangeset-api-openapi.yml
  format: yaml
  label: Amazon Marketplace StartChangeSet API
  slug: amazon-marketplace-startchangeset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-startchangeset-api-openapi.yml
- filename: amazon-marketplace-tagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace TagResource API
  slug: amazon-marketplace-tagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-tagresource-api-openapi.yml
- filename: amazon-marketplace-untagresource-api-openapi.yml
  format: yaml
  label: Amazon Marketplace UntagResource API
  slug: amazon-marketplace-untagresource-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/openapi/amazon-marketplace-untagresource-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: catalog.marketplace.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Marketplace, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
slug: amazon-marketplace-domain-security
source_filename: amazon-marketplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: catalog.marketplace.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/security/amazon-marketplace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
---
