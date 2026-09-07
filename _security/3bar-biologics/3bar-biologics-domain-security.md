---
api_specs:
- filename: 3bar-biologics-posts-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Posts API
  slug: 3bar-biologics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-posts-api-openapi.yml
- filename: 3bar-biologics-pages-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Pages API
  slug: 3bar-biologics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-pages-api-openapi.yml
- filename: 3bar-biologics-media-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Media API
  slug: 3bar-biologics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-media-api-openapi.yml
- filename: 3bar-biologics-taxonomy-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Taxonomy API
  slug: 3bar-biologics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-taxonomy-api-openapi.yml
- filename: 3bar-biologics-users-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Users API
  slug: 3bar-biologics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-users-api-openapi.yml
- filename: 3bar-biologics-search-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Search API
  slug: 3bar-biologics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-search-api-openapi.yml
- filename: 3bar-biologics-discovery-api-openapi.yml
  format: yaml
  label: 3Bar Biologics Discovery API
  slug: 3bar-biologics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-discovery-api-openapi.yml
- filename: 3bar-biologics-oembed-api-openapi.yml
  format: yaml
  label: 3Bar Biologics oEmbed API
  slug: 3bar-biologics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-oembed-api-openapi.yml
- filename: 3bar-biologics-seo-api-openapi.yml
  format: yaml
  label: 3Bar Biologics SEO Metadata API
  slug: 3bar-biologics-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/openapi/3bar-biologics-seo-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3barbiologics.com
  spf: true
hosts:
- cert_expires: Oct 21 15:20:23 2026 GMT
  host: www.3barbiologics.com
  hsts: true
  hsts_max_age: 300
  hsts_note: 300 seconds is five minutes. The RFC 6797 preload threshold and common practice is 31536000 (one year); a five-minute max-age gives a returning visitor essentially no protection against an SSL-stripping downgrade, because the policy has almost always expired between visits. This is the Pantheon platform default for a site that has not enabled full HSTS.
  https: true
  tls_version: TLSv1.3
- host: 3barbiologics.com
  hsts: null
  https: false
  https_error: tls-certificate-name-mismatch
  note: The apex domain is broken over HTTPS. It resolves to Pantheon (23.185.0.2) but the certificate presented is CN=pantheonsite.io, whose SANs are *.getpantheon.com, *.gotpantheon.com, *.pantheon.io, *.pantheonsite.io, getpantheon.com, gotpantheon.com and pantheonsite.io — none of which covers 3barbiologics.com. Every browser shows a certificate warning. Plain HTTP to the apex returns 404 rather than redirecting to www, so there is no working path from `3barbiologics.com` to the site by either scheme. A visitor who types the domain without `www.` does not reach 3Bar Biologics.
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 3Bar Biologics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3Bar Biologics, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3Bar Biologics
provider_slug: 3bar-biologics
slug: 3bar-biologics-domain-security
source_filename: 3bar-biologics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3barbiologics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 15:20:23 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  hsts_note: >-\n    300 seconds is five minutes. The RFC 6797 preload threshold and common practice is 31536000 (one\n    year); a five-minute max-age gives a returning visitor essentially no protection against an\n    SSL-stripping downgrade, because the policy has almost always expired between visits. This is\n    the Pantheon platform default for a site that has not enabled full HSTS.\n- host: 3barbiologics.com\n  https: false\n  https_error: tls-certificate-name-mismatch\n  hsts: null\n  note: >-\n    The apex domain is broken over HTTPS. It resolves to Pantheon (23.185.0.2) but the certificate\n    presented is CN=pantheonsite.io, whose SANs are *.getpantheon.com, *.gotpantheon.com,\n    *.pantheon.io, *.pantheonsite.io,\
  \ getpantheon.com, gotpantheon.com and pantheonsite.io — none of\n    which covers 3barbiologics.com. Every browser shows a certificate warning. Plain HTTP to the\n    apex returns 404 rather than redirecting to www, so there is no working path from\n    `3barbiologics.com` to the site by either scheme. A visitor who types the domain without `www.`\n    does not reach 3Bar Biologics.\ndomains:\n- domain: 3barbiologics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\nfindings:\n- id: apex-tls-mismatch\n  severity: high\n  summary: The apex domain serves a certificate that does not cover it, and does not redirect on HTTP.\n  detail: >-\n    https://3barbiologics.com/ fails the TLS handshake with a name mismatch; http://3barbiologics.com/\n    returns 404 with no Location header. Only https://www.3barbiologics.com/ works.\n  evidence:\n  - {url: 'https://3barbiologics.com/', http_status: 0, error: certificate name mismatch (CN=pantheonsite.io)}\n  - {url: 'http://3barbiologics.com/',\
  \ http_status: 404, redirect_url: null}\n  - {url: 'https://www.3barbiologics.com/', http_status: 200}\n  remediation_owner: provider\n- id: preproduction-hostname-leak\n  severity: medium\n  summary: >-\n    The production homepage hard-codes 79 absolute URLs pointing at Pantheon platform hostnames,\n    including the site's only Privacy Policy link.\n  detail: >-\n    www.3barbiologics.com serves HTML containing 26 absolute links to\n    https://dev-3bar-biologics.pantheonsite.io and 53 to https://live-3bar-biologics.pantheonsite.io.\n    The dev host is reachable, returns 200, and serves the same WordPress REST API as production —\n    it is a pre-production environment exposed to the public internet and linked to from the\n    production site. The Privacy Policy link in the page footer points at\n    https://dev-3bar-biologics.pantheonsite.io/privacy-policy/ rather than at the canonical\n    www.3barbiologics.com/privacy-policy/, which does exist and returns 200. Font assets are also\n\
  \    loaded cross-origin from the live-* platform host.\n  consequence: >-\n    Visitors following the Privacy Policy link land on an unbranded platform hostname. Search engines\n    and AI crawlers see duplicate content on three hostnames, splitting canonical signal. Anything\n    staged on the dev environment is publicly readable, including through its own REST API.\n  evidence:\n  - {url: 'https://www.3barbiologics.com/', http_status: 200, finding: '26 dev-* and 53 live-* absolute pantheonsite.io URLs in the served HTML'}\n  - {url: 'https://dev-3bar-biologics.pantheonsite.io/privacy-policy/', http_status: 200, finding: 'the target of the production footer Privacy Policy link'}\n  - {url: 'https://dev-3bar-biologics.pantheonsite.io/wp-json/', http_status: 200, finding: 'the pre-production environment serves the same REST API'}\n  - {url: 'https://www.3barbiologics.com/privacy-policy/', http_status: 200, finding: 'the canonical page exists and is not the one linked'}\n  remediation_owner:\
  \ provider\n- id: no-dmarc\n  severity: medium\n  summary: SPF is published but DMARC is not.\n  detail: >-\n    An SPF record exists for 3barbiologics.com, but there is no _dmarc TXT record, so there is no\n    policy telling receivers what to do with mail that fails authentication and no reporting channel.\n    The company publishes a sales address (Sales@3BarBiologics.com) on its site, which is the address\n    a spoofing campaign would impersonate.\n  remediation_owner: provider\n- id: no-dnssec-no-caa\n  severity: low\n  summary: Neither DNSSEC nor CAA is configured for 3barbiologics.com.\n  detail: >-\n    No DNSSEC signing and no CAA record restricting which certificate authorities may issue for the\n    domain. Both are common absences and neither is exploitable on its own.\n  remediation_owner: provider\n- id: hsts-max-age-300\n  severity: low\n  summary: HSTS is present on www but expires after five minutes.\n  detail: See the hsts_note on the www host above.\n  remediation_owner:\
  \ provider\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3bar-biologics/refs/heads/main/security/3bar-biologics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Agricultural Biologicals
- Biomanufacturing
- CDMO
- Microbials
- Crop Inputs
- Sustainability
- Contract Manufacturing
- Content
---
