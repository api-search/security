---
api_specs:
- filename: centrexion-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Comments API
  slug: centrexion-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-comments-api-openapi.yml
- filename: centrexion-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Custom Types API
  slug: centrexion-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-custom-types-api-openapi.yml
- filename: centrexion-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Discovery API
  slug: centrexion-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-discovery-api-openapi.yml
- filename: centrexion-therapeutics-media-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Media API
  slug: centrexion-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-media-api-openapi.yml
- filename: centrexion-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Oembed API
  slug: centrexion-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-oembed-api-openapi.yml
- filename: centrexion-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Pages API
  slug: centrexion-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-pages-api-openapi.yml
- filename: centrexion-therapeutics-people-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics People API
  slug: centrexion-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-people-api-openapi.yml
- filename: centrexion-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Posts API
  slug: centrexion-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-posts-api-openapi.yml
- filename: centrexion-therapeutics-search-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Search API
  slug: centrexion-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-search-api-openapi.yml
- filename: centrexion-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Taxonomy API
  slug: centrexion-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: centrexion.com
  nameservers:
  - dns101.register.com
  - dns102.register.com
  spf: true
  spf_record: v=spf1 include:1xalkvunf.spf.checkpoint-spf.com -all
hosts:
- cert_expires: Oct 23 21:24:08 2026 GMT
  host: centrexion.com
  hsts: false
  http_to_https_redirect: 301
  https: true
  origin: WP Engine (x-powered-by response header observed)
  server: nginx
  tls_version: TLSv1.3
  www_redirect: 301 to apex
kind: domain-security
layout: security
method: probed
name: Centrexion Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrexion Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Centrexion Therapeutics
provider_slug: centrexion-therapeutics
slug: centrexion-therapeutics-domain-security
source_filename: centrexion-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the centrexion.com host and registrable domain\nnote: >-\n  Probed 2026-08-09 by the API Evangelist enrichment pipeline. Only Centrexion Therapeutics' own\n  host and registrable domain are recorded. The apis.yml humanURL for the content API points at\n  developer.wordpress.org (the upstream WordPress REST handbook that documents the wp/v2 contract);\n  that host is not operated by Centrexion and its posture is deliberately excluded so it is not\n  misattributed to this provider. The site is a WordPress deployment served by nginx and hosted on\n  WP Engine (x-powered-by: WP Engine). HTTPS is enforced by redirect (http:// and www. both 301 to\n  https://centrexion.com/) but no Strict-Transport-Security header is sent, so the redirect is the\n  only downgrade protection. No CAA records and no DNSSEC are published; DNS is delegated to\n  Register.com.\nhosts:\n- host: centrexion.com\n  https: true\n \
  \ tls_version: TLSv1.3\n  cert_expires: Oct 23 21:24:08 2026 GMT\n  hsts: false\n  server: nginx\n  origin: WP Engine (x-powered-by response header observed)\n  http_to_https_redirect: 301\n  www_redirect: 301 to apex\ndomains:\n- domain: centrexion.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:1xalkvunf.spf.checkpoint-spf.com -all'\n  dmarc: false\n  nameservers:\n  - dns101.register.com\n  - dns102.register.com\nobservations:\n- >-\n  No DMARC record is published at _dmarc.centrexion.com (empty TXT response). SPF is present and\n  strict (-all, delegated to Check Point's hosted email-security SPF service), but with no DMARC\n  policy there is no alignment enforcement and no aggregate or forensic reporting, so the domain has\n  neither spoofing enforcement beyond SPF nor any visibility into abuse.\n- >-\n  DANGLING CNAME — investors.centrexion.com is a CNAME to centrexion.gcs-web.com, and that target\n  has no A record while its parent zone gcs-web.com is\
  \ live on AWS Route 53 nameservers. The name\n  therefore resolves as a CNAME but terminates in NXDOMAIN, and nothing answers on 80 or 443. A\n  CNAME left pointing at a de-provisioned host on a third-party investor-relations platform is the\n  classic subdomain-takeover precondition; whoever can claim that hostname on the upstream platform\n  inherits a subdomain of centrexion.com. Recommend deleting the record or reclaiming the target.\n- >-\n  portal.centrexion.com resolves to 72.20.122.198 but both 443 and 80 are closed/filtered — a stale\n  A record for a host that no longer serves. sharepoint.centrexion.com (66.227.71.31) behaves the\n  same way. Neither is a live surface; both are residue.\n- No Strict-Transport-Security header on the site root.\n- No Content-Security-Policy header on the site root.\n- No X-Content-Type-Options, X-Frame-Options, Referrer-Policy or Permissions-Policy header on the site root.\n- >-\n  API responses under /wp-json do send x-content-type-options nosniff\
  \ and x-robots-tag noindex, and\n  expose Access-Control-Expose-Headers for X-WP-Total, X-WP-TotalPages and Link.\n- No /.well-known/security.txt (RFC 9116) published — see well-known/centrexion-therapeutics-well-known.yml.\n- >-\n  No api., developer., docs., status., trust., mcp., support., vpn., intranet., files. or careers.\n  subdomain resolves for centrexion.com (NXDOMAIN on all eleven), consistent with a company that\n  runs no developer program and no status or trust surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/security/centrexion-therapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biopharmaceutical
- Pharmaceuticals
- Chronic Pain
- non-opioid-analgesics
- Immunology
- inflammation
- Clinical Trials
- Life Sciences
- content-api
---
