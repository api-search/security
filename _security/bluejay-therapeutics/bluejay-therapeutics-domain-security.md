---
api_specs:
- filename: bluejay-therapeutics-content-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Content API
  slug: bluejay-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-content-api-openapi.yml
- filename: bluejay-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Discovery API
  slug: bluejay-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-discovery-api-openapi.yml
- filename: bluejay-therapeutics-embed-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Embed API
  slug: bluejay-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-embed-api-openapi.yml
- filename: bluejay-therapeutics-empty-collections-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Empty Collections API
  slug: bluejay-therapeutics-empty-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-empty-collections-api-openapi.yml
- filename: bluejay-therapeutics-media-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Media API
  slug: bluejay-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-media-api-openapi.yml
- filename: bluejay-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Taxonomy API
  slug: bluejay-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bluejaytx.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Oct 23 23:23:52 2026 GMT
  host: bluejaytx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluejay Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluejay Therapeutics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Bluejay Therapeutics
provider_slug: bluejay-therapeutics
slug: bluejay-therapeutics-domain-security
source_filename: bluejay-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluejaytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:23:52 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: bluejaytx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/security/bluejay-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- biopharmaceuticals
- Pharmaceuticals
- Life Sciences
- hepatology
- Infectious Disease
- Clinical Trials
- Drug Development
- Monoclonal Antibodies
- content-api
---
