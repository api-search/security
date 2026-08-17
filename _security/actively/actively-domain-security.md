---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: actively.ai
  spf: true
hosts:
- cert_expires: Sep 19 06:39:55 2026 GMT
  host: www.actively.ai
  hsts: true
  hsts_max_age: 0
  https: true
  note: Framer/Cloudflare-hosted marketing site. HSTS header is PRESENT but with max-age=0, which disables it — effectively no HSTS.
  tls_version: TLSv1.3
- cert_expires: Nov 11 17:47:22 2026 GMT
  host: api.actively.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: The API host (Google Frontend) carries a materially stronger header set than the marketing site — two-year HSTS with includeSubDomains, plus a full CSP and cross-origin isolation set.
  security_headers:
  - content-security-policy: default-src 'self'; frame-ancestors 'none';
  - x-frame-options: DENY
  - x-content-type-options: nosniff
  - referrer-policy: strict-origin-when-cross-origin
  - cross-origin-opener-policy: same-origin
  - cross-origin-embedder-policy: require-corp
  tls_version: TLSv1.3
- host: auth.actively.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Authorization server (WorkOS AuthKit on Actively's custom domain). One-year HSTS with includeSubDomains and preload.
- host: trust.actively.ai
  hsts: null
  https: true
  note: Vanta-hosted trust center on the company's own subdomain.
kind: domain-security
layout: security
method: probed
name: Actively Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actively, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Actively
provider_slug: actively
slug: actively-domain-security
source_filename: actively-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + discovery hosts\nhosts:\n- host: www.actively.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 06:39:55 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n  note: >-\n    Framer/Cloudflare-hosted marketing site. HSTS header is PRESENT but with\n    max-age=0, which disables it — effectively no HSTS.\n- host: api.actively.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 17:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  security_headers:\n  - content-security-policy: \"default-src 'self'; frame-ancestors 'none';\"\n  - x-frame-options: DENY\n  - x-content-type-options: nosniff\n  - referrer-policy: strict-origin-when-cross-origin\n  - cross-origin-opener-policy: same-origin\n  - cross-origin-embedder-policy: require-corp\n  note: >-\n    The API host (Google Frontend) carries a materially stronger header set\n    than the\
  \ marketing site — two-year HSTS with includeSubDomains, plus a\n    full CSP and cross-origin isolation set.\n- host: auth.actively.ai\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: >-\n    Authorization server (WorkOS AuthKit on Actively's custom domain).\n    One-year HSTS with includeSubDomains and preload.\n- host: trust.actively.ai\n  https: true\n  hsts: null\n  note: Vanta-hosted trust center on the company's own subdomain.\ndomains:\n- domain: actively.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- >-\n  DNSSEC is not enabled on actively.ai.\n- >-\n  No CAA records are published, so any public CA may issue for the domain.\n- >-\n  DMARC exists but the policy is p=none — monitoring only, no enforcement\n  against spoofed mail.\n- >-\n  HSTS is inconsistent across the estate: strong on api.actively.ai\n  (max-age=63072000) and auth.actively.ai (preloaded), but\
  \ max-age=0 on\n  www.actively.ai, which turns it off for the primary domain.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actively/refs/heads/main/security/actively-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- AI Agents
- Revenue Intelligence
- Sales
- Go To Market
- MCP
- OAuth
- Model Context Protocol
- Sales Intelligence
- Enterprise Software
---
