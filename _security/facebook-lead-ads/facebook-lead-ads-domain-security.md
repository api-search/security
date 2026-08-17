---
api_specs:
- filename: facebook-lead-ads-bulk-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Bulk Leads API
  slug: facebook-lead-ads-bulk-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-bulk-leads-api-openapi.yml
- filename: facebook-lead-ads-leadgen-forms-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leadgen Forms API
  slug: facebook-lead-ads-leadgen-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leadgen-forms-api-openapi.yml
- filename: facebook-lead-ads-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leads API
  slug: facebook-lead-ads-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leads-api-openapi.yml
- filename: facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Meta Marketing API Lead Ads API
  slug: facebook-lead-ads-meta-marketing-api-lead-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
- filename: facebook-lead-ads-subscribed-apps-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscribed Apps API
  slug: facebook-lead-ads-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscribed-apps-api-openapi.yml
- filename: facebook-lead-ads-subscriptions-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscriptions API
  slug: facebook-lead-ads-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  caa_note: CAA is present and account-pinned — issuance is restricted to a single DigiCert account, which is stricter than a bare issuer-name CAA.
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; rua=mailto:a@dmarc.facebookmail.com; ruf=mailto:fb-dmarc@datafeeds.phishlabs.com; pct=100
  dnssec: false
  dnssec_note: No DNSKEY record returned.
  domain: facebook.com
  spf: true
  spf_record: v=spf1 redirect=_spf.facebook.com
hosts:
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: graph.facebook.com
  hsts: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  role: Graph API base
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: developers.facebook.com
  hsts: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  role: developer portal / documentation
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: www.facebook.com
  hsts: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  role: OAuth authorization dialog + OIDC discovery
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: mcp.facebook.com
  hsts: true
  hsts_max_age: 15552000
  hsts_preload: true
  https: true
  role: Meta-hosted Ads MCP server
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facebook Lead Ads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facebook Lead Ads, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Facebook Lead Ads
provider_slug: facebook-lead-ads
slug: facebook-lead-ads-domain-security
source_filename: facebook-lead-ads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live TLS handshake + HEAD request per host, and dig for the registrable domain\nnote: >-\n  Probed by hand rather than by 0-working/probe-domain-security.py. That script's shared\n  provider_hosts() helper excludes facebook.com as a social-media link, which is correct for\n  the other ~9,000 providers in the catalog but wrong here, where facebook.com IS the API\n  domain. Results below are direct observations taken 2026-08-14.\nhosts:\n  - host: graph.facebook.com\n    role: Graph API base\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: 'Aug 21 23:59:59 2026 GMT'\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_preload: true\n  - host: developers.facebook.com\n    role: developer portal / documentation\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: 'Aug 21 23:59:59 2026 GMT'\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_preload: true\n  - host: www.facebook.com\n    role: OAuth authorization\
  \ dialog + OIDC discovery\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: 'Aug 21 23:59:59 2026 GMT'\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_preload: true\n  - host: mcp.facebook.com\n    role: Meta-hosted Ads MCP server\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: 'Aug 21 23:59:59 2026 GMT'\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_preload: true\ndomains:\n  - domain: facebook.com\n    dnssec: false\n    dnssec_note: No DNSKEY record returned.\n    caa:\n      - '0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"'\n    caa_note: >-\n      CAA is present and account-pinned — issuance is restricted to a single DigiCert\n      account, which is stricter than a bare issuer-name CAA.\n    spf: true\n    spf_record: 'v=spf1 redirect=_spf.facebook.com'\n    dmarc: true\n    dmarc_policy: reject\n    dmarc_record: >-\n      v=DMARC1; p=reject; rua=mailto:a@dmarc.facebookmail.com;\n      ruf=mailto:fb-dmarc@datafeeds.phishlabs.com;\
  \ pct=100\nsummary:\n  hosts_probed: 4\n  https: 4/4\n  tls13: 4/4\n  hsts: 4/4\n  hsts_preload: 4/4\n  dnssec: false\n  caa: true\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  gaps: [dnssec]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/security/facebook-lead-ads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhooks
---
