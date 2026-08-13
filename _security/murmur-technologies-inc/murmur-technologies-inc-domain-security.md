---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: murmurcars.com
  mx: true
  mx_provider: Google Workspace
  nameservers: AWS Route 53
  note: Google Workspace mail is still configured (MX present) but no SPF, DMARC, CAA, or DNSSEC records are published. An unauthenticated sender can spoof this domain.
  spf: false
  txt:
  - google-site-verification=VenwwoNIDt3-D5TjmucHV0We9RcWy8n3z0NhYhfPMmE
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none;
  dnssec: false
  domain: murmurads.com
  mx: true
  mx_provider: Google Workspace
  nameservers: AWS Route 53
  note: 'Better configured than murmurcars.com but still permissive: the SPF record ends in `?all` (neutral) rather than `-all` or `~all`, and DMARC is set to `p=none`, which monitors without quarantining or rejecting. Neither CAA nor DNSSEC is published.'
  spf: true
  spf_policy: neutral
  spf_record: v=spf1 include:sendersrv.com ?all
hosts:
- a_record: true
  cname: d2yeufc603kica.cloudfront.net
  csp: false
  host: portal.murmurads.com
  hsts: false
  https: true
  note: Live static single-page app; index.html last modified 2024-12-26. TLS terminates at CloudFront. No security headers are set on the origin.
  reachable: true
  server: AmazonS3 via CloudFront
  tls:
    issuer: C=US, O=Amazon, CN=Amazon RSA 2048 M04
    not_after: '2026-11-05'
    not_before: '2025-10-07'
    subject: CN=*.murmurads.com
    valid: true
    wildcard: true
  x_frame_options: false
- a_record: true
  host: backendapp.murmurcars.com
  https: false
  ip: 34.222.140.165
  note: The API host the portal's JavaScript bundle calls. Resolves, but TCP 443 and 80 are filtered/dead and every request times out. TLS could not be negotiated.
  reachable: false
- a_record: false
  host: murmurcars.com
  https: false
  note: apex has Route 53 NS but no A record; no reachable HTTPS host.
  reachable: false
- a_record: false
  host: murmurads.com
  https: false
  note: apex has Route 53 NS but no A record; no reachable HTTPS host.
  reachable: false
- a_record: true
  host: blog.murmurcars.com
  https: false
  ip: 18.209.59.200
  note: resolves but times out on 443.
  reachable: false
kind: domain-security
layout: security
method: probed
name: Murmur Technologies Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Murmur Technologies INC, probed live across 5 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Murmur Technologies INC
provider_slug: murmur-technologies-inc
slug: murmur-technologies-inc-domain-security
source_filename: murmur-technologies-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  dig DNS probe of murmurcars.com and murmurads.com, plus openssl s_client TLS\n  and curl header probe of portal.murmurads.com (the only Murmur host that\n  answers HTTPS).\nnote: >-\n  Supersedes the 2026-07-20 probe, which concluded no host was reachable and so\n  could not test TLS at all. A reachable host has since been found:\n  portal.murmurads.com, the advertiser portal, serves over HTTPS from Amazon S3\n  behind CloudFront with a valid Amazon-issued wildcard certificate for\n  *.murmurads.com. TLS itself is sound (CloudFront default), but the origin\n  publishes NO security response headers — no HSTS, no CSP, no X-Frame-Options.\n  At the DNS layer both apex domains remain dark: neither murmurcars.com nor\n  murmurads.com carries an A record, and neither publishes CAA or DNSSEC.\n  Email posture differs between the two domains and is recorded separately\n  below: murmurads.com publishes SPF and DMARC, murmurcars.com\
  \ publishes\n  neither. The certificate was reissued 2025-10-07 and Google Workspace MX is\n  live on both domains, so the registrations are still being maintained even\n  though the public web presence is down.\nhosts:\n  - host: portal.murmurads.com\n    https: true\n    reachable: true\n    a_record: true\n    cname: d2yeufc603kica.cloudfront.net\n    tls:\n      valid: true\n      subject: CN=*.murmurads.com\n      issuer: 'C=US, O=Amazon, CN=Amazon RSA 2048 M04'\n      not_before: '2025-10-07'\n      not_after: '2026-11-05'\n      wildcard: true\n    hsts: false\n    csp: false\n    x_frame_options: false\n    server: AmazonS3 via CloudFront\n    note: >-\n      Live static single-page app; index.html last modified 2024-12-26. TLS\n      terminates at CloudFront. No security headers are set on the origin.\n  - host: backendapp.murmurcars.com\n    https: false\n    reachable: false\n    a_record: true\n    ip: 34.222.140.165\n    note: >-\n      The API host the portal's JavaScript\
  \ bundle calls. Resolves, but TCP 443\n      and 80 are filtered/dead and every request times out. TLS could not be\n      negotiated.\n  - host: murmurcars.com\n    https: false\n    reachable: false\n    a_record: false\n    note: apex has Route 53 NS but no A record; no reachable HTTPS host.\n  - host: murmurads.com\n    https: false\n    reachable: false\n    a_record: false\n    note: apex has Route 53 NS but no A record; no reachable HTTPS host.\n  - host: blog.murmurcars.com\n    https: false\n    reachable: false\n    a_record: true\n    ip: 18.209.59.200\n    note: resolves but times out on 443.\ndomains:\n  - domain: murmurcars.com\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n    dmarc_policy: null\n    mx: true\n    mx_provider: Google Workspace\n    nameservers: AWS Route 53\n    txt:\n      - google-site-verification=VenwwoNIDt3-D5TjmucHV0We9RcWy8n3z0NhYhfPMmE\n    note: >-\n      Google Workspace mail is still configured (MX present) but no SPF, DMARC,\n\
  \      CAA, or DNSSEC records are published. An unauthenticated sender can spoof\n      this domain.\n  - domain: murmurads.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:sendersrv.com ?all'\n    spf_policy: neutral\n    dmarc: true\n    dmarc_policy: none\n    dmarc_record: 'v=DMARC1; p=none;'\n    mx: true\n    mx_provider: Google Workspace\n    nameservers: AWS Route 53\n    note: >-\n      Better configured than murmurcars.com but still permissive: the SPF record\n      ends in `?all` (neutral) rather than `-all` or `~all`, and DMARC is set to\n      `p=none`, which monitors without quarantining or rejecting. Neither CAA\n      nor DNSSEC is published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/murmur-technologies-inc/refs/heads/main/security/murmur-technologies-inc-domain-security.yml
summary_line: DMARC
tags:
- Company
- Advertising
- AdTech
- Out-of-Home Advertising
- Digital Billboards
- Mobile Advertising
- Marketing
---
