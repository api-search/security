---
api_specs:
- filename: amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Auto Scaling Group API
  slug: amazon-ec2-auto-scaling-auto-scaling-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-auto-scaling-group-api-openapi.yml
- filename: amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Launch Configuration API
  slug: amazon-ec2-auto-scaling-launch-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-launch-configuration-api-openapi.yml
- filename: amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Lifecycle Hook API
  slug: amazon-ec2-auto-scaling-lifecycle-hook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-lifecycle-hook-api-openapi.yml
- filename: amazon-ec2-auto-scaling-load-balancer-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Load Balancer API
  slug: amazon-ec2-auto-scaling-load-balancer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-load-balancer-api-openapi.yml
- filename: amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Load Balancer Target Group API
  slug: amazon-ec2-auto-scaling-load-balancer-target-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-load-balancer-target-group-api-openapi.yml
- filename: amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Notification Configuration API
  slug: amazon-ec2-auto-scaling-notification-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-notification-configuration-api-openapi.yml
- filename: amazon-ec2-auto-scaling-operations-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Operations API
  slug: amazon-ec2-auto-scaling-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-operations-api-openapi.yml
- filename: amazon-ec2-auto-scaling-policy-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Policy API
  slug: amazon-ec2-auto-scaling-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-policy-api-openapi.yml
- filename: amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Scaling Plan API
  slug: amazon-ec2-auto-scaling-scaling-plan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-scaling-plan-api-openapi.yml
- filename: amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Scheduled Action API
  slug: amazon-ec2-auto-scaling-scheduled-action-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-scheduled-action-api-openapi.yml
- filename: amazon-ec2-auto-scaling-traffic-source-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Traffic Source API
  slug: amazon-ec2-auto-scaling-traffic-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-traffic-source-api-openapi.yml
- filename: amazon-ec2-auto-scaling-warm-pool-api-openapi.yml
  format: yaml
  label: Amazon EC2 Auto Scaling Ec2 Auto Scaling Warm Pool API
  slug: amazon-ec2-auto-scaling-warm-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ec2-auto-scaling/openapi/amazon-ec2-auto-scaling-warm-pool-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: autoscaling.amazonaws.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon EC2 Auto Scaling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon EC2 Auto Scaling, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
slug: amazon-ec2-auto-scaling-domain-security
source_filename: amazon-ec2-auto-scaling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: autoscaling.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-ec2-auto-scaling/security/amazon-ec2-auto-scaling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Auto-Scaling
- Compute
- EC2
- High Availability
- Scaling
---
