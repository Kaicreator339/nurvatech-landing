# DNS Setup for www.nurvatech.com

## GitHub Pages Deployment
- **Repo:** https://github.com/Kaicreator339/nurvatech-landing
- **Status:** Building (check in 1-2 minutes)
- **URL:** https://Kaicreator339.github.io/nurvatech-landing
- **Custom domain:** www.nurvatech.com (configured)

## Namecheap DNS Records

Add these records in Namecheap DNS management:

### A Records (IPv4)
```
Type: A
Host: @
Value: 185.199.108.153
TTL: Automatic

Type: A  
Host: @
Value: 185.199.109.153
TTL: Automatic

Type: A
Host: @
Value: 185.199.110.153
TTL: Automatic

Type: A
Host: @
Value: 185.199.111.153
TTL: Automatic
```

### CNAME Record
```
Type: CNAME
Host: www
Value: Kaicreator339.github.io
TTL: Automatic
```

## Verification Steps

1. **Wait 5-10 minutes** after adding DNS records
2. **Check site:** https://www.nurvatech.com
3. **GitHub Pages status:** Should show "Published"
4. **SSL:** GitHub provides free SSL automatically (may take up to 24h)

## Email Setup (Already Configured)
- **ImprovMX:** info@nurvatech.com → nurvatech@gmail.com
- **Verify:** Send test email to info@nurvatech.com

## Troubleshooting
- **DNS propagation:** Can take up to 48h globally
- **GitHub Pages build:** Check Actions tab in repo
- **Custom domain:** Verify in repo Settings → Pages
- **SSL:** May show "Not Secure" initially, wait for auto-provisioning

## Quick Test Commands
```bash
# Check DNS
dig www.nurvatech.com
dig nurvatech.com

# Check GitHub Pages
curl -I https://Kaicreator339.github.io/nurvatech-landing
```