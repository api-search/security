---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_raw: v=DMARC1; p=quarantine; adkim=r; aspf=r; rua=mailto:dmarc_rua@onsecureserver.net;
  dnssec: false
  domain: trycardinal.com
  note: 'Weaker than the .ai domain on two counts: no CAA records at all, and a DMARC policy of quarantine rather than reject. This is now the primary brand domain, so the weaker posture applies to the name customers see.'
  registrar_dns: framer / sites.framer.app
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
- caa:
  - 0 iodef "mailto:jianna@trycardinal.ai"
  - 0 issue "starfieldtech.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_raw: v=DMARC1; p=reject; adkim=r; aspf=r; rua=mailto:dmarc_rua@onsecureserver.net;
  dnssec: false
  domain: trycardinal.ai
  note: CAA is present and names a founder's address as the incident contact (mailto:jianna@trycardinal.ai) — a real, human-owned iodef target. Since the prior pass (2026-07-21) two issuers were added alongside Let's Encrypt (starfieldtech.com and godaddy.com), widening the set of CAs permitted to issue for this domain. DMARC is at p=reject, the strongest published policy across either domain.
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Oct 27 23:25:25 2026 GMT
  host: www.trycardinal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: marketing website (Framer-hosted)
  tls_version: TLSv1.3
- cert_expires: Feb 14 16:12:24 2027 GMT
  host: trycardinal.ai
  hsts: true
  hsts_max_age: 31536000
  http_status: 301
  https: true
  note: Root 301s to the .com marketing site. Deep paths that existed on the old site (/company, /product) now return HTTP 404, so this is a root-only redirect rather than a path-preserving domain migration.
  redirects_to: https://www.trycardinal.com/
  role: legacy marketing domain — 301 redirect
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:49:59 2026 GMT
  final_url: https://app.trycardinal.ai/login?next=%2F
  host: app.trycardinal.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
  note: 'The strongest security posture of the three hosts: a full CSP with an explicit allow-list, frame-ancestors ''none'', two-year HSTS with includeSubDomains, and nosniff. Every unauthenticated path redirects to a Stytch-backed login.'
  role: customer application (Next.js on Vercel)
  security_headers:
    content_security_policy: true
    frame_ancestors: none
    permissions_policy: camera=(), microphone=(), geolocation=()
    referrer_policy: strict-origin-when-cross-origin
    x_content_type_options: nosniff
    x_frame_options: DENY
  tls_version: TLSv1.3
- dns_cname: coordinator-api-wmxp.onrender.com
  host: api.trycardinal.ai
  http_body: 'error code: 1001'
  http_status: 409
  https: false
  note: A DEAD CUSTOM DOMAIN, recorded because its absence is the finding. DNS resolves api.trycardinal.ai to a Render service (coordinator-api-wmxp.onrender.com), but no TLS certificate covers the custom hostname, so every HTTPS request fails at the handshake; plain HTTP returns Cloudflare error 1001 (HTTP 409). Probing the Render origin directly returns HTTP 404 with x-render-routing:no-server on every path, which is Render's response when no service is attached. Nothing is served here, and no API host is asserted anywhere in this repo on the strength of this record.
  origin_probe:
    header: 'x-render-routing: no-server'
    status: 404
    url: https://coordinator-api-wmxp.onrender.com/
  role: custom API hostname — NOT SERVING
  tls_error: SSLV3_ALERT_HANDSHAKE_FAILURE — no certificate is presented for this name
kind: domain-security
layout: security
method: probed
name: Trycardinal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardinal, probed live across 4 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardinal
provider_slug: trycardinal-ai
slug: trycardinal-ai-domain-security
source_filename: trycardinal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of every host associated with Cardinal. The marketing host\n  came from probe-domain-security.py (which reads the apis.yml Website pointer); the\n  three trycardinal.ai hosts were probed by hand in the same pass and merged in,\n  because apis.yml carries no apis[] entries and no baseURL, so the script's host\n  discovery only reaches the website domain. Both registrable domains are covered.\nchecked: '2026-08-13'\n\nhosts:\n- host: www.trycardinal.com\n  role: marketing website (Framer-hosted)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:25:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n\n- host: trycardinal.ai\n  role: legacy marketing domain — 301 redirect\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 16:12:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  http_status: 301\n  redirects_to: https://www.trycardinal.com/\n  note: >-\n    Root 301s\
  \ to the .com marketing site. Deep paths that existed on the old site\n    (/company, /product) now return HTTP 404, so this is a root-only redirect rather\n    than a path-preserving domain migration.\n\n- host: app.trycardinal.ai\n  role: customer application (Next.js on Vercel)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:49:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  http_status: 200\n  final_url: https://app.trycardinal.ai/login?next=%2F\n  security_headers:\n    content_security_policy: true\n    x_frame_options: DENY\n    x_content_type_options: nosniff\n    referrer_policy: strict-origin-when-cross-origin\n    permissions_policy: camera=(), microphone=(), geolocation=()\n    frame_ancestors: none\n  note: >-\n    The strongest security posture of the three hosts: a full CSP with an explicit\n    allow-list, frame-ancestors 'none', two-year HSTS with includeSubDomains, and\n    nosniff. Every unauthenticated path redirects\
  \ to a Stytch-backed login.\n\n- host: api.trycardinal.ai\n  role: custom API hostname — NOT SERVING\n  https: false\n  tls_error: 'SSLV3_ALERT_HANDSHAKE_FAILURE — no certificate is presented for this name'\n  http_status: 409\n  http_body: 'error code: 1001'\n  dns_cname: coordinator-api-wmxp.onrender.com\n  origin_probe:\n    url: https://coordinator-api-wmxp.onrender.com/\n    status: 404\n    header: 'x-render-routing: no-server'\n  note: >-\n    A DEAD CUSTOM DOMAIN, recorded because its absence is the finding. DNS resolves\n    api.trycardinal.ai to a Render service (coordinator-api-wmxp.onrender.com), but no\n    TLS certificate covers the custom hostname, so every HTTPS request fails at the\n    handshake; plain HTTP returns Cloudflare error 1001 (HTTP 409). Probing the Render\n    origin directly returns HTTP 404 with x-render-routing:no-server on every path,\n    which is Render's response when no service is attached. Nothing is served here, and\n    no API host is asserted anywhere\
  \ in this repo on the strength of this record.\n\ndomains:\n- domain: trycardinal.com\n  registrar_dns: framer / sites.framer.app\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_raw: 'v=DMARC1; p=quarantine; adkim=r; aspf=r; rua=mailto:dmarc_rua@onsecureserver.net;'\n  note: >-\n    Weaker than the .ai domain on two counts: no CAA records at all, and a DMARC policy\n    of quarantine rather than reject. This is now the primary brand domain, so the\n    weaker posture applies to the name customers see.\n\n- domain: trycardinal.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:jianna@trycardinal.ai\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_raw: 'v=DMARC1; p=reject; adkim=r; aspf=r; rua=mailto:dmarc_rua@onsecureserver.net;'\n  note:\
  \ >-\n    CAA is present and names a founder's address as the incident contact\n    (mailto:jianna@trycardinal.ai) — a real, human-owned iodef target. Since the prior\n    pass (2026-07-21) two issuers were added alongside Let's Encrypt (starfieldtech.com\n    and godaddy.com), widening the set of CAs permitted to issue for this domain.\n    DMARC is at p=reject, the strongest published policy across either domain.\n\nsummary:\n  hosts_probed: 4\n  hosts_serving_https: 3\n  domains_probed: 2\n  dnssec_enabled: 0\n  dmarc_enforced: 2\n  caa_present: 1\n  weakest_link: >-\n    trycardinal.com — the primary brand domain — has no CAA records and only\n    p=quarantine DMARC, while the legacy trycardinal.ai domain has both. Neither domain\n    signs DNSSEC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trycardinal-ai/refs/heads/main/security/trycardinal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Outbound Sales
- Sales Automation
- Sales Engagement
- Go-To-Market
- Revenue Operations
- AI Agents
- Lead Generation
- Machine-Learning
---
