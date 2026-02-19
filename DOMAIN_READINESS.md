# NurvaTech Domain Readiness Plan

## Domain Strategy
**Core principle:** All services domain-first, no localhost dependencies.

## Immediate Domain-Based Services

### 1. Client Portal (Ready for DNS)
- **URL:** https://clients.nurvatech.com (subdomain)
- **Purpose:** Client dashboard, project tracking, file sharing
- **Tech:** GitHub Pages + HTML/CSS/JS
- **Status:** Can build immediately

### 2. Service Catalog
- **URL:** https://services.nurvatech.com
- **Purpose:** Detailed service offerings, pricing, case studies
- **Tech:** Static site (free hosting)
- **Status:** Ready to build

### 3. OpenClaw Demo
- **URL:** https://demo.nurvatech.com
- **Purpose:** Interactive OpenClaw capabilities showcase
- **Tech:** GitHub Pages with interactive examples
- **Status:** Design phase

## DNS-Ready Infrastructure

### Subdomains to Configure (Once DNS Working):
```
clients.nurvatech.com   → Client portal
services.nurvatech.com  → Service catalog  
demo.nurvatech.com      → Interactive demo
blog.nurvatech.com      → Technical blog
status.nurvatech.com    → System status
```

### Email Infrastructure:
- **Primary:** info@nurvatech.com (ImprovMX → Gmail)
- **Sales:** sales@nurvatech.com (forward to same)
- **Support:** support@nurvatech.com (forward to same)

## Phase 1: Build While DNS Pending

### Week 1 Goals:
1. ✅ Main landing page (done)
2. 🔄 Client portal MVP
3. 🔄 Service catalog
4. 🔄 Basic blog framework

### Technology Stack (All Free):
- **Hosting:** GitHub Pages, Netlify, Vercel
- **Email:** ImprovMX (free tier)
- **Analytics:** Plausible (free for personal)
- **Forms:** Tally.so (free forms)

## Marketing/Sales Preparation

### Ready for DNS:
1. **LinkedIn Company Page** draft
2. **Twitter/X account** setup
3. **Initial content calendar**
4. **Case study templates**
5. **Proposal templates**

### Lead Generation:
- **Landing page forms** (Tally.so)
- **Email newsletter signup**
- **Consultation booking system**

## Monitoring Setup

### DNS Watchdog:
```bash
# Cron job to check when DNS propagates
#!/bin/bash
if curl -s https://www.nurvatech.com > /dev/null; then
  echo "DNS LIVE - Activating full deployment"
  # Trigger all domain services
fi
```

### Automated Tasks (When DNS Live):
1. Enable all subdomains
2. Activate monitoring
3. Start SSL provisioning checks
4. Launch marketing sequences

## Next 24h Actions

### While You're Away:
1. Build client portal MVP
2. Create service catalog
3. Draft marketing materials
4. Set up monitoring scripts

### When DNS Configured (5 min task):
1. Add subdomain DNS records
2. Deploy all prepared services
3. Activate monitoring
4. Begin outreach

## Success Metrics
- **DNS to live:** < 1 hour after configuration
- **Full suite deployed:** < 4 hours after DNS
- **First lead capture:** < 24h after launch
- **Cost:** $0 (all free services)

## Risk Mitigation
- **No local dependencies:** All services cloud-hosted
- **Progressive enhancement:** Start simple, add features
- **Automated deployment:** One-click updates
- **Monitoring:** Instant alerts if anything breaks