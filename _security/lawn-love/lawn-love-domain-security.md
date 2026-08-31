---
description: ''
domains: []
hosts:
- headers:
    cache_control: no-cache, private
    cookies_samesite: lax
    cookies_secure: true
  host: lawnlove.com
  hsts:
    evidence: no strict-transport-security header on the apex response
    present: false
  tls:
    application: laravel-vapor
    certificate_verified: true
    edge: cloudflare
    evidence: 'HTTP/2 200 over TLS with ssl_verify_result=0; response carries server: cloudflare and x-vapor-base64-encode headers'
    https: true
- headers:
    access_control_allow_origin: '*'
    referrer_policy: strict-origin-when-cross-origin
    x_content_type_options: nosniff
    x_frame_options: SAMEORIGIN
  host: api.lawnlove.com
  hsts:
    evidence: 'strict-transport-security: max-age=300; includeSubDomains'
    include_subdomains: true
    max_age: 300
    note: max-age of 300 seconds is far below the 31536000 (1 year) commonly recommended for preload-eligible HSTS
    present: true
  tls:
    certificate_verified: true
    edge: cloudflare + aws-cloudfront + api-gateway
    evidence: 'response headers include x-amz-apigw-id, via 1.1 ... cloudfront.net, and server: cloudflare'
    https: true
kind: domain-security
layout: security
method: probed
name: Lawn Love Domain Security
name_suffix: Domain Security
overview: Domain security posture for Lawn Love, probed live across 2 host(s) and 0 registrable domain(s).
provider_name: Lawn Love
provider_slug: lawn-love
slug: lawn-love-domain-security
source_filename: lawn-love-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig + curl probes of lawnlove.com and api.lawnlove.com\ndomain: lawnlove.com\nhosts:\n- host: lawnlove.com\n  tls:\n    https: true\n    certificate_verified: true\n    edge: cloudflare\n    application: laravel-vapor\n    evidence: >-\n      HTTP/2 200 over TLS with ssl_verify_result=0; response carries\n      server: cloudflare and x-vapor-base64-encode headers\n  hsts:\n    present: false\n    evidence: no strict-transport-security header on the apex response\n  headers:\n    cache_control: 'no-cache, private'\n    cookies_secure: true\n    cookies_samesite: lax\n- host: api.lawnlove.com\n  tls:\n    https: true\n    certificate_verified: true\n    edge: cloudflare + aws-cloudfront + api-gateway\n    evidence: >-\n      response headers include x-amz-apigw-id, via 1.1 ... cloudfront.net,\n      and server: cloudflare\n  hsts:\n    present: true\n    max_age: 300\n    include_subdomains: true\n    evidence: 'strict-transport-security:\
  \ max-age=300; includeSubDomains'\n    note: >-\n      max-age of 300 seconds is far below the 31536000 (1 year) commonly\n      recommended for preload-eligible HSTS\n  headers:\n    x_frame_options: SAMEORIGIN\n    x_content_type_options: nosniff\n    referrer_policy: strict-origin-when-cross-origin\n    access_control_allow_origin: '*'\ndns:\n  nameservers:\n  - sara.ns.cloudflare.com\n  - mitch.ns.cloudflare.com\n  a_records:\n  - 172.66.174.91\n  - 104.20.32.191\n  dnssec:\n    enabled: false\n    evidence: no DS record returned for lawnlove.com\n  caa:\n    present: false\n    evidence: no CAA records returned for lawnlove.com\nemail:\n  spf:\n    present: true\n    record: 'v=spf1 include:sendgrid.net include:_spf.google.com include:servers.mcsv.net include:mail.zendesk.com ~all'\n    policy: softfail\n    senders:\n    - sendgrid.net\n    - _spf.google.com\n    - servers.mcsv.net\n    - mail.zendesk.com\n  dmarc:\n    present: true\n    record: 'v=DMARC1; p=none; rua=mailto:media@lawnlove.com'\n\
  \    policy: none\n    aggregate_reports: media@lawnlove.com\n    note: >-\n      p=none is monitor-only and does not instruct receivers to quarantine or\n      reject spoofed mail\nfindings:\n- severity: low\n  finding: No DNSSEC (no DS record published).\n- severity: low\n  finding: No CAA record, so any public CA may issue for the domain.\n- severity: low\n  finding: No HSTS on the apex host; api.lawnlove.com sets only max-age=300.\n- severity: low\n  finding: DMARC policy is p=none (monitoring only, no enforcement).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lawn-love/refs/heads/main/security/lawn-love-domain-security.yml
summary_line: HSTS
tags:
- Company
- Home Services
- Lawn Care
- Marketplace
- On Demand
- Field Service
- Scheduling
- Local Services
- Consumer
---
