---
description: ''
domains:
- a_records:
  - 35.208.4.74
  caa: []
  caa_note: no CAA record published, so any CA may issue for this domain
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; fo=1; rua=mailto:REDACTED@rep.dmarcanalyzer.com; ruf=mailto:REDACTED@for.dmarcanalyzer.com;
  dnssec: false
  dnssec_evidence: no DS record at the parent and no RRSIG on the A response
  domain: viridos.com
  mx:
  - 10 us-smtp-inbound-1.mimecast.com
  - 20 us-smtp-inbound-2.mimecast.com
  nameservers:
  - dns1.easydns.com
  - dns2.easydns.net
  - dns3.easydns.ca
  observation: Mail posture is strong and still live - Mimecast inbound gateways, Microsoft 365 sending, SPF hard-fail, DMARC p=reject with aggregate and forensic reporting - while the web presence is gone entirely. This is the fingerprint of a wound-down company whose DNS and mail tenancy outlived its website.
  spf: true
  spf_policy: -all
  spf_record: v=spf1 include:spf.protection.outlook.com include:us._netblocks.mimecast.com include:spfus.rocketseed.com include:_spf.atlassian.net include:_spf.psm.knowbe4.com -all
- a_records:
  - 13.32.241.2
  - 13.32.241.16
  - 13.32.241.38
  - 13.32.241.117
  domain: dspace.bio
  http_status: 403
  note: The public demo host named in the company's own sgidspace README. Still resolves to AWS CloudFront (13.32.241.0/24) but every path returns 403; the distribution no longer serves the D-SPACE demo.
hosts:
- cert_covers_host: false
  cert_expires: Sep 27 07:42:30 2026 GMT
  cert_issuer: C=US, O=Let's Encrypt, CN=YR1
  cert_subject: CN=giowm1252.siteground.biz
  host: viridos.com
  hsts: null
  hsts_note: no Strict-Transport-Security header is returned; the host serves no site to protect
  http_body: 403 | Access blocked
  http_status: 403
  https: false
  https_note: TLS handshake succeeds (TLSv1.3, TLS_AES_256_GCM_SHA384) but the certificate does not cover viridos.com - subject CN=giowm1252.siteground.biz, issuer Let's Encrypt, valid 2026-06-29 to 2026-09-27 - so a verifying client fails with a name mismatch.
  response_headers:
    server: nginx
    sg-captcha: challenge
    x-default-vhost: '1'
    x-robots-tag: noindex
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synthetic Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viridos, probed live across 1 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Viridos
provider_slug: synthetic-genomics
slug: synthetic-genomics-domain-security
source_filename: synthetic-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the company's own domain (viridos.com), 2026-08-29\nnote: >-\n  The first automated run of probe-domain-security.py profiled forgeglobal.com, because the only\n  host named anywhere in apis.yml was a Forge Global secondary-market listing page. Forge Global is\n  a trading venue, not Viridos, so that result has been replaced with a probe of the company's own\n  domain. DNS and mail for viridos.com are still fully configured and enterprise-grade, but no web\n  vhost is served: every HTTP path returns \"403 | Access blocked\" from a SiteGround default vhost,\n  behind a certificate issued for giowm1252.siteground.biz rather than for viridos.com.\nhosts:\n- host: viridos.com\n  https: false\n  https_note: >-\n    TLS handshake succeeds (TLSv1.3, TLS_AES_256_GCM_SHA384) but the certificate does not cover\n    viridos.com - subject CN=giowm1252.siteground.biz, issuer Let's Encrypt, valid\n    2026-06-29\
  \ to 2026-09-27 - so a verifying client fails with a name mismatch.\n  tls_version: TLSv1.3\n  cert_subject: CN=giowm1252.siteground.biz\n  cert_issuer: \"C=US, O=Let's Encrypt, CN=YR1\"\n  cert_expires: Sep 27 07:42:30 2026 GMT\n  cert_covers_host: false\n  http_status: 403\n  http_body: '403 | Access blocked'\n  response_headers:\n    server: nginx\n    sg-captcha: challenge\n    x-robots-tag: noindex\n    x-default-vhost: '1'\n  hsts: null\n  hsts_note: no Strict-Transport-Security header is returned; the host serves no site to protect\ndomains:\n- domain: viridos.com\n  a_records:\n  - 35.208.4.74\n  nameservers:\n  - dns1.easydns.com\n  - dns2.easydns.net\n  - dns3.easydns.ca\n  dnssec: false\n  dnssec_evidence: no DS record at the parent and no RRSIG on the A response\n  caa: []\n  caa_note: no CAA record published, so any CA may issue for this domain\n  spf: true\n  spf_record: >-\n    v=spf1 include:spf.protection.outlook.com include:us._netblocks.mimecast.com\n    include:spfus.rocketseed.com\
  \ include:_spf.atlassian.net include:_spf.psm.knowbe4.com -all\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: >-\n    v=DMARC1; p=reject; fo=1; rua=mailto:REDACTED@rep.dmarcanalyzer.com;\n    ruf=mailto:REDACTED@for.dmarcanalyzer.com;\n  mx:\n  - 10 us-smtp-inbound-1.mimecast.com\n  - 20 us-smtp-inbound-2.mimecast.com\n  observation: >-\n    Mail posture is strong and still live - Mimecast inbound gateways, Microsoft 365 sending,\n    SPF hard-fail, DMARC p=reject with aggregate and forensic reporting - while the web presence\n    is gone entirely. This is the fingerprint of a wound-down company whose DNS and mail tenancy\n    outlived its website.\n- domain: dspace.bio\n  note: >-\n    The public demo host named in the company's own sgidspace README. Still resolves to AWS\n    CloudFront (13.32.241.0/24) but every path returns 403; the distribution no longer serves\n    the D-SPACE demo.\n  a_records:\n  - 13.32.241.2\n  - 13.32.241.16\n  - 13.32.241.38\n\
  \  - 13.32.241.117\n  http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthetic-genomics/refs/heads/main/security/synthetic-genomics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Synthetic Biology
- Biotechnology
- Genomics
- Biofuels
- Algae
- Climate Tech
- Life Sciences
- Open Source
- Defunct
---
