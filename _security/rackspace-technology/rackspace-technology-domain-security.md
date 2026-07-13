---
api_specs:
- filename: rackspace-cloud-dns.yaml
  format: yaml
  label: Rackspace Cloud DNS API
  slug: cloud-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-cloud-dns.yaml
- filename: rackspace-customer-service.yaml
  format: yaml
  label: Rackspace Customer Service API
  slug: customer-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-customer-service.yaml
- filename: rackspace-cloud-identity.yaml
  format: yaml
  label: Rackspace Customer Identity API
  slug: customer-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-cloud-identity.yaml
- filename: rackspace-offer.yaml
  format: yaml
  label: Rackspace Offer API
  slug: offer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/openapi/rackspace-offer.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rackspace.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rackspacecloud.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.rackspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 17 17:26:44 2026 GMT
  host: docs.rackspace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: dns.api.rackspacecloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rackspace Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rackspace Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rackspace Technology
provider_slug: rackspace-technology
slug: rackspace-technology-domain-security
source_filename: rackspace-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rackspace.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.rackspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:26:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dns.api.rackspacecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rackspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rackspacecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rackspace-technology/refs/heads/main/security/rackspace-technology-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cloud
- Managed Services
- Multicloud
- Infrastructure
- DevOps
---
