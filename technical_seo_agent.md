# TECHNICAL SEO AGENT

**Role:** Technical SEO Auditor & Site Health Engineer

**Expertise:** Crawlability, indexing, Core Web Vitals, site speed, structured data

---

## Technical SEO Audit Checklist

### Sitemap & Robots
- [ ] Sitemap.xml exists and is submitted to GSC
- [ ] Robots.txt properly configured
- [ ] No important URLs blocked in robots.txt
- [ ] Sitemap includes all important URLs
- [ ] Sitemap URLs use canonical paths
- [ ] Images included in sitemap
- [ ] Update frequency set correctly

**Robots.txt Template:**
```
User-agent: *
Allow: /
Disallow: /admin/
Disallow: /private/
Disallow: /temp/

Sitemap: https://volarktiles.com/sitemap.xml
```

### Core Web Vitals
- [ ] Largest Contentful Paint (LCP) < 2.5 seconds
- [ ] First Input Delay (FID) < 100 milliseconds
- [ ] Cumulative Layout Shift (CLS) < 0.1
- [ ] Desktop score 90+
- [ ] Mobile score 90+
- [ ] Page Speed Insights checked monthly

**Improvement Actions:**
- Optimize images (compression, lazy loading)
- Minimize CSS/JS
- Use CDN for fast delivery
- Enable browser caching
- Defer non-critical JS

### Broken Links & Redirects
- [ ] No 404 errors on important pages
- [ ] 301 redirects for moved content
- [ ] No redirect chains (→ → → avoid)
- [ ] No redirect loops
- [ ] External links to authoritative sites
- [ ] Internal links all working
- [ ] Remove orphan pages or link them

**Monitoring:**
- Weekly: Check crawl errors in GSC
- Monthly: Run full site crawl
- Quarterly: Review redirect audit

### Canonicals
- [ ] Self-referential canonicals on all pages
- [ ] Correct canonical (not to homepage)
- [ ] HTTPS canonicals (not HTTP)
- [ ] Consistent canonical across versions
- [ ] No canonical chains
- [ ] Parameters handled properly

**Example:**
```html
<link rel="canonical" href="https://volarktiles.com/porcelain-tiles/">
```

### Indexability
- [ ] Crawl errors resolved
- [ ] No pages blocked by robots.txt
- [ ] No noindex tags on important pages
- [ ] GSC coverage: 95%+ indexed
- [ ] URL parameters managed (UTM, session IDs)
- [ ] Mobile version indexable
- [ ] No noindex on pagination

**GSC Coverage Issues to Fix:**
- Excluded (robots.txt)
- Not indexed (crawl errors)
- Submitted but not indexed (quality issues)

### Canonicals & Duplicates
- [ ] No duplicate content across pages
- [ ] Canonical tags handle variations
- [ ] HTTP vs HTTPS handled
- [ ] WWW vs non-WWW consistent
- [ ] Trailing slashes consistent
- [ ] Parameter canonicals used

**Fix Strategy:**
```
1. Redirect duplicates to canonical
2. Add canonical tag
3. Update internal links
4. Resubmit to GSC
```

### Mobile Optimization
- [ ] Mobile-first indexing ready
- [ ] Mobile viewport set correctly
- [ ] Touch-friendly buttons (48x48px minimum)
- [ ] No Flash or plugins
- [ ] Font sizes readable (16px minimum)
- [ ] No pop-ups covering content
- [ ] Links spaced properly
- [ ] Images responsive

**Meta Tag:**
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### SSL/HTTPS
- [ ] HTTPS enabled on all pages
- [ ] SSL certificate valid (not expired)
- [ ] Redirect HTTP → HTTPS
- [ ] Mixed content fixed (http content on https page)
- [ ] Certificate covers all domains
- [ ] No SSL warnings

---

## Core Web Vitals Optimization

### LCP (Largest Contentful Paint) - First Visual Change
**Goal:** < 2.5 seconds

**Causes of Slow LCP:**
- Large images not optimized
- Render-blocking CSS/JS
- Slow server response (TTFB)
- Client-side rendering delays

**Fixes:**
```
1. Image Optimization
   - Compress all images (tools: TinyPNG, ImageOptim)
   - Use WebP format
   - Lazy load below-fold images
   - Serve correct image sizes

2. Reduce CSS/JS
   - Remove unused CSS
   - Minify CSS/JavaScript
   - Inline critical CSS
   - Defer non-critical JavaScript

3. Server Response
   - Upgrade hosting if slow
   - Use CDN (Cloudflare, Akamai)
   - Enable caching headers
   - Optimize database queries
```

### CLS (Cumulative Layout Shift) - Visual Stability
**Goal:** < 0.1 (no jumping elements)

**Common Issues:**
- Images without fixed dimensions
- Ads/embeds without reserved space
- Fonts loading and changing size
- Dynamic content added above fold

**Fixes:**
```
1. Reserve Space
   - Set width/height on images
   - Reserve space for ads
   - Specify font metrics

2. Avoid Late Loads
   - Don't inject content above fold
   - Keep ads below fold
   - Use stable font loading
```

---

## Monthly Technical Audit Template

```
AUDIT DATE: [Date]
SITE: volarktiles.com

1. CRAWLABILITY
   - Crawl errors: [X]
   - Blocked URLs: [X]
   - Redirect issues: [X]
   Status: [PASS/FAIL]

2. INDEXABILITY
   - Total indexed: [X]
   - Coverage: [X%]
   - Noindex issues: [X]
   Status: [PASS/FAIL]

3. CORE WEB VITALS
   - LCP: [X]s
   - FID: [X]ms
   - CLS: [X]
   - Score: [X/100]
   Status: [PASS/FAIL]

4. SECURITY
   - SSL valid: YES/NO
   - No malware: YES/NO
   - Status: [PASS/FAIL]

5. MOBILE
   - Mobile friendly: YES/NO
   - Usable: YES/NO
   Status: [PASS/FAIL]

RECOMMENDATIONS:
1. [Fix most critical issue]
2. [Fix second priority]
3. [Monitor metric]

NEXT AUDIT: [Date]
```

---

## Common Issues & Quick Fixes

| Issue | Impact | Fix | Priority |
|-------|--------|-----|----------|
| Slow LCP | CRITICAL | Optimize images, minify CSS | URGENT |
| Crawl errors | HIGH | Fix broken links, 404s | HIGH |
| Missing robots.txt | MEDIUM | Create proper robots.txt | HIGH |
| Poor mobile UX | HIGH | Fix layout, touch targets | HIGH |
| Expired SSL | CRITICAL | Renew certificate | URGENT |
| 404 pages | MEDIUM | Redirect or fix links | MEDIUM |
| Mixed content | MEDIUM | Convert HTTP → HTTPS | MEDIUM |
| Slow TTFB | HIGH | Upgrade hosting/use CDN | HIGH |

---

## Tools & Monitoring

### Free Tools
- Google PageSpeed Insights
- Google Search Console
- Google Mobile-Friendly Test
- Lighthouse (browser built-in)
- GTmetrix (free version)

### Monitoring Strategy
```
Daily: Check GSC for new crawl errors
Weekly: Monitor Core Web Vitals
Monthly: Full technical audit
Quarterly: Comprehensive security check
```

---

## Success Metrics

- ✅ Zero critical crawl errors
- ✅ 95%+ GSC coverage
- ✅ Core Web Vitals all green (>90 score)
- ✅ Page speed < 2 seconds
- ✅ Mobile speed < 3 seconds
- ✅ TTFB < 600ms
- ✅ Zero SSL/security warnings

---

## Notes

- Technical SEO = foundation (necessary but not sufficient)
- Speed matters more each year (is ranking factor)
- Mobile-first is now standard
- Structured data increasingly important
- Security (SSL) now required for all sites
- Crawlability issues are easy wins (fix them first)
