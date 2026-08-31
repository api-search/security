---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:postmaster@stepful.com; pct=100; adkim=s; aspf=s
  dnssec: false
  domain: stepful.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Oct  7 23:52:27 2026 GMT
  cert_valid: true
  host: www.stepful.com
  hsts: false
  https: true
  operator: stepful
  role: marketing site (Webflow)
  server: cloudflare
  tls_version: TLSv1.3
- cert_valid: true
  host: classroom.stepful.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  operator: stepful
  role: authenticated student learning application (Rails/Devise)
  server: cloudflare
  tls_version: TLSv1.3
- cert_valid: true
  host: admin.stepful.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  operator: stepful
  role: authenticated staff admin application (Rails/Devise)
  server: Heroku
  tls_version: TLSv1.3
- cert_valid: true
  host: asset-cdn.stepful.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  operator: stepful
  role: static asset CDN (CloudFront)
  server: cloudflare
  tls_version: TLSv1.3
- cert_valid: true
  csp: true
  host: c.stepful.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  operator: third-party (Converge, runconverge.com)
  role: first-party-domain analytics/attribution proxy; CNAME dqhzqrkt8v2js.cloudfront.net
  tls_version: TLSv1.3
  x_content_type_options: nosniff
  x_frame_options: DENY
- host: k.stepful.com
  https: true
  operator: third-party (PostHog)
  role: product-analytics reverse proxy; CNAME d4f93c1a51f965c39c9e.cf-prod-us-proxy.proxyhog.com
kind: domain-security
layout: security
method: probed
name: Stepful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stepful, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Stepful
provider_slug: stepful
slug: stepful-domain-security
source_filename: stepful-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every stepful.com host discovered during enrichment\nnote: >-\n  Stepful publishes no API host. The hosts below are its marketing site (Webflow behind\n  Cloudflare), its authenticated student classroom and staff admin applications, its asset\n  CDN, and two vendor subdomains CNAME'd to third parties (c.stepful.com -> Converge /\n  runconverge.com, k.stepful.com -> PostHog / proxyhog.com). Vendor-operated hosts are\n  recorded for completeness but their posture is the vendor's, not Stepful's.\nhosts:\n- host: www.stepful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  cert_expires: 'Oct  7 23:52:27 2026 GMT'\n  hsts: false\n  server: cloudflare\n  operator: stepful\n  role: marketing site (Webflow)\n- host: classroom.stepful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: cloudflare\n\
  \  operator: stepful\n  role: authenticated student learning application (Rails/Devise)\n- host: admin.stepful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: Heroku\n  operator: stepful\n  role: authenticated staff admin application (Rails/Devise)\n- host: asset-cdn.stepful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  server: cloudflare\n  operator: stepful\n  role: static asset CDN (CloudFront)\n- host: c.stepful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_valid: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  csp: true\n  x_frame_options: DENY\n  x_content_type_options: nosniff\n  operator: third-party (Converge, runconverge.com)\n  role: first-party-domain analytics/attribution proxy; CNAME dqhzqrkt8v2js.cloudfront.net\n- host: k.stepful.com\n  https: true\n\
  \  operator: third-party (PostHog)\n  role: product-analytics reverse proxy; CNAME d4f93c1a51f965c39c9e.cf-prod-us-proxy.proxyhog.com\ndomains:\n- domain: stepful.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com ~all'\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:postmaster@stepful.com; pct=100; adkim=s; aspf=s'\nfindings:\n- No CAA record is published for stepful.com, so any public CA may issue for the domain.\n- DNSSEC is not enabled on stepful.com.\n- DMARC is published but at p=none, so no enforcement action is requested of receivers.\n- The apex marketing host www.stepful.com does not send HSTS, while every application host does.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepful/refs/heads/main/security/stepful-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Healthcare
- Workforce Development
- Online Learning
- Certification
- Allied Health
- Career Training
- Staffing
- EdTech
---
