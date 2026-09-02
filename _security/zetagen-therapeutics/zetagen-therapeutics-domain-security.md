---
api_specs:
- filename: zetagen-therapeutics-content-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Content API
  slug: zetagen-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-content-api-openapi.yml
- filename: zetagen-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Discovery API
  slug: zetagen-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-discovery-api-openapi.yml
- filename: zetagen-therapeutics-downloads-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Downloads API
  slug: zetagen-therapeutics-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-downloads-api-openapi.yml
- filename: zetagen-therapeutics-embed-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Embed API
  slug: zetagen-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-embed-api-openapi.yml
- filename: zetagen-therapeutics-media-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Media API
  slug: zetagen-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-media-api-openapi.yml
- filename: zetagen-therapeutics-people-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics People API
  slug: zetagen-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-people-api-openapi.yml
- filename: zetagen-therapeutics-search-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Search API
  slug: zetagen-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-search-api-openapi.yml
- filename: zetagen-therapeutics-seo-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Seo API
  slug: zetagen-therapeutics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-seo-api-openapi.yml
- filename: zetagen-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Zetagen Therapeutics Taxonomy API
  slug: zetagen-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/openapi/zetagen-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; pct=100; rua=mailto:a.yoylfgnf@sdmarc.net
  dnssec: false
  domain: zetagen.com
  note: DMARC is at full enforcement (p=reject, pct=100) and both SPF and DMARC are delegated to a managed service (sdmarc.net) — the strongest single signal in this profile. No CAA records and no DNSSEC.
  spf: true
  spf_record: v=spf1 redirect=_syoylfgnf.sdmarc.net
hosts:
- cert_expires: Oct 26 08:36:11 2026 GMT
  host: zetagen.com
  hsts: false
  http3: true
  https: true
  note: alt-svc advertises h3, h3-29 and several draft QUIC versions. No Strict-Transport-Security header on the site root or on /wp-json responses. API responses carry x-content-type-options nosniff and x-robots-tag noindex.
  server: LiteSpeed
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zetagen Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zetagen Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zetagen Therapeutics
provider_slug: zetagen-therapeutics
slug: zetagen-therapeutics-domain-security
source_filename: zetagen-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the zetagen.com host on 2026-08-05\nnote: >-\n  Only zetagen.com is Zetagen Therapeutics' own host. The mechanical probe also walked\n  developer.wordpress.org because that URL is the API's humanURL — the upstream WordPress REST\n  handbook that defines the wp/v2 contract — but that domain belongs to the WordPress Foundation and\n  its posture says nothing about this provider, so it is recorded separately below and excluded from\n  the provider assessment. No api./developer./docs./status./trust. subdomain of zetagen.com resolves.\nhosts:\n- host: zetagen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:36:11 2026 GMT\n  hsts: false\n  server: LiteSpeed\n  http3: true\n  note: >-\n    alt-svc advertises h3, h3-29 and several draft QUIC versions. No Strict-Transport-Security\n    header on the site root or on /wp-json responses. API responses carry x-content-type-options\n    nosniff\
  \ and x-robots-tag noindex.\ndomains:\n- domain: zetagen.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 redirect=_syoylfgnf.sdmarc.net\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; pct=100; rua=mailto:a.yoylfgnf@sdmarc.net'\n  note: >-\n    DMARC is at full enforcement (p=reject, pct=100) and both SPF and DMARC are delegated to a\n    managed service (sdmarc.net) — the strongest single signal in this profile. No CAA records and\n    no DNSSEC.\nnon_provider_hosts:\n- host: developer.wordpress.org\n  domain: wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    WordPress Foundation infrastructure, reached only because it is the\
  \ API's humanURL. Not\n    operated by Zetagen Therapeutics; recorded for transparency, not scored against this provider.\nsubdomains_probed:\n- {host: api.zetagen.com, resolves: false}\n- {host: developer.zetagen.com, resolves: false}\n- {host: docs.zetagen.com, resolves: false}\n- {host: status.zetagen.com, resolves: false}\n- {host: trust.zetagen.com, resolves: false}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zetagen-therapeutics/refs/heads/main/security/zetagen-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- biopharmaceuticals
- Oncology
- Bone Health
- Orthopedics
- Clinical Trials
- Life Sciences
- Drug Development
- Medical Devices
- content-api
---
