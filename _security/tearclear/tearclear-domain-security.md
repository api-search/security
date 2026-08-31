---
description: ''
domains: []
hosts:
- assessment: 'Email is live and conventionally configured (Microsoft 365 MX, SPF with -all, DMARC at p=none), but the web presence is not: the domain resolves to SiteGround shared hosting where it is not provisioned as a virtual host, so every request falls to the default vhost and is refused with 403 under a certificate for another name. No DNSSEC, no CAA, no HSTS.'
  dns:
    a:
    - 35.215.120.120
    caa: false
    caa_evidence: no CAA record returned for tearclear.com
    dmarc: true
    dmarc_note: p=none is monitor-only; it publishes a DMARC record but instructs receivers to take no action on failures.
    dmarc_policy: none
    dmarc_record: v=DMARC1; p=none; aspf=r; adkim=r;
    dnssec: false
    dnssec_evidence: no DNSKEY record returned for tearclear.com
    mx:
    - tearclear-com.mail.protection.outlook.com
    ns:
    - ns07.domaincontrol.com
    - ns08.domaincontrol.com
    spf: true
    spf_record: v=spf1 include:spf.protection.outlook.com -all
  host: tearclear.com
  https:
    certificate:
      covers_host: false
      hostname_mismatch: The certificate presented for tearclear.com carries only DNS:gcam1074.siteground.biz in its SAN list, so any client verifying the hostname fails the handshake. curl returns error 60 without -k.
      issuer: Let's Encrypt
      not_after: '2026-10-27'
      not_before: '2026-07-29'
      subject_cn: gcam1074.siteground.biz
    hsts: false
    hsts_evidence: no Strict-Transport-Security header on the 403 response
    http_status: 403
    reachable: true
    response_headers_of_note:
      sg-captcha: challenge
      x-default-vhost: '1'
      x-robots-tag: noindex
    server: nginx
    tls_cipher: TLS_AES_256_GCM_SHA384
    tls_protocol: TLSv1.3
  probed: '2026-08-29'
kind: domain-security
layout: security
method: probed
name: Tearclear Domain Security
name_suffix: Domain Security
overview: Domain security posture for Tearclear, probed live across 1 host(s) and 0 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS.
provider_name: Tearclear
provider_slug: tearclear
slug: tearclear-domain-security
source_filename: tearclear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: tearclear.com (DNS + TLS live probe)\nnote: >-\n  Probed by hand rather than by probe-domain-security.py, because that script reads hosts\n  only from a `Website`/`Portal` pointer in apis.yml and this repo intentionally carries no\n  Website pointer: tearclear.com does not serve. Absence of a record is valid data.\nhosts:\n- host: tearclear.com\n  probed: '2026-08-29'\n  dns:\n    a:\n    - 35.215.120.120\n    ns:\n    - ns07.domaincontrol.com\n    - ns08.domaincontrol.com\n    mx:\n    - tearclear-com.mail.protection.outlook.com\n    dnssec: false\n    dnssec_evidence: no DNSKEY record returned for tearclear.com\n    caa: false\n    caa_evidence: no CAA record returned for tearclear.com\n    spf: true\n    spf_record: v=spf1 include:spf.protection.outlook.com -all\n    dmarc: true\n    dmarc_record: 'v=DMARC1; p=none; aspf=r; adkim=r;'\n    dmarc_policy: none\n    dmarc_note: >-\n      p=none is monitor-only; it publishes a\
  \ DMARC record but instructs receivers to take\n      no action on failures.\n  https:\n    reachable: true\n    http_status: 403\n    tls_protocol: TLSv1.3\n    tls_cipher: TLS_AES_256_GCM_SHA384\n    certificate:\n      subject_cn: gcam1074.siteground.biz\n      issuer: \"Let's Encrypt\"\n      not_before: '2026-07-29'\n      not_after: '2026-10-27'\n      covers_host: false\n      hostname_mismatch: >-\n        The certificate presented for tearclear.com carries only\n        DNS:gcam1074.siteground.biz in its SAN list, so any client verifying the hostname\n        fails the handshake. curl returns error 60 without -k.\n    hsts: false\n    hsts_evidence: no Strict-Transport-Security header on the 403 response\n    server: nginx\n    response_headers_of_note:\n      x-default-vhost: '1'\n      sg-captcha: challenge\n      x-robots-tag: noindex\n  assessment: >-\n    Email is live and conventionally configured (Microsoft 365 MX, SPF with -all, DMARC at\n    p=none), but the web presence\
  \ is not: the domain resolves to SiteGround shared hosting\n    where it is not provisioned as a virtual host, so every request falls to the default\n    vhost and is refused with 403 under a certificate for another name. No DNSSEC, no CAA,\n    no HSTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tearclear/refs/heads/main/security/tearclear-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Pharmaceuticals
- Ophthalmology
- Drug Delivery
- Life Sciences
- Medical Devices
- Glaucoma
- Clinical Stage
---
