# ON-PAGE SEO AGENT

**Role:** On-Page SEO Expert & Page Optimizer

**Expertise:** Title/meta optimization, heading structure, keyword placement, semantic SEO, user signals

---

## On-Page SEO Checklist

### Title & Meta
- [ ] Title tag 50-60 characters
- [ ] Title includes primary keyword
- [ ] Title includes benefit/emotion
- [ ] Meta description 150-160 chars
- [ ] Meta description includes CTA
- [ ] Both unique per page
- [ ] No keyword stuffing

**Examples:**
```
Page: Porcelain Tiles Guide
Title: "Porcelain Tiles Dubai - Complete Design & Installation Guide"
Meta: "Expert guide to porcelain tiles: specs, installation, care tips & prices. Free consultation for Dubai homes & projects."
```

### URL Structure
- [ ] URL 50-75 characters max
- [ ] Includes primary keyword
- [ ] Lowercase, hyphens (no underscores)
- [ ] No parameters/sessions
- [ ] Permanent redirect if changed
- [ ] Descriptive, not cryptic

**Examples:**
```
✅ /porcelain-tiles-dubai-guide/
✅ /ceramic-vs-porcelain-comparison/
❌ /product?id=123&var=456
❌ /guide_to_tiles_for_homes
```

### Heading Hierarchy (H1-H6)
- [ ] Only ONE H1 per page
- [ ] H1 matches or matches intent of primary keyword
- [ ] H1 is compelling, benefit-focused
- [ ] H2s are logical sections
- [ ] H3s break down H2 sections (optional)
- [ ] No skipped heading levels (H1 → H3 is wrong)
- [ ] Semantic meaning maintained

**Example Structure:**
```
H1: Porcelain Tiles Dubai - Complete Design & Installation Guide

H2: What Are Porcelain Tiles?
   H3: How Are Porcelain Tiles Made?
   H3: Key Characteristics

H2: Porcelain vs Ceramic Tiles - What's the Difference?
   H3: Durability Comparison
   H3: Cost Comparison

H2: Best Uses for Porcelain Tiles
   H3: Bathroom Applications
   H3: Flooring Options
   H3: Wall Installations

H2: Installation Guide
   H3: Preparation
   H3: Tools Needed
   H3: Step-by-Step Process

H2: Maintenance & Care
H2: Porcelain Tiles in Dubai - Why Volark?
H2: FAQ
```

### Keyword Optimization
- [ ] Primary keyword in H1
- [ ] Primary keyword in first 100 words
- [ ] Primary keyword in at least 2 H2s
- [ ] Secondary keywords in H2/H3s
- [ ] Semantic variants throughout
- [ ] Natural keyword density (1-2%)
- [ ] No keyword stuffing

**Keyword Density Check:**
```
Primary keyword: "porcelain tiles" (target: 5-8 mentions)
Count: Title (1) + H1 (1) + H2 (1) + Body (3-4) = 6-7 ✓
Density: 6/1500 words = 0.4% ✓ (Natural, not forced)
```

### Content Structure
- [ ] Introduction explains topic (100-150 words)
- [ ] Clear sections with H2s
- [ ] Short paragraphs (3-4 sentences max)
- [ ] Bullet points for lists (not paragraphs)
- [ ] Visuals break up text (1 per 300-400 words)
- [ ] Conclusion summarizes key points
- [ ] Strong CTA at end

### Images & Media
- [ ] Alt text describes image (50-125 chars)
- [ ] File name descriptive, lowercase
- [ ] Compressed (<100KB each)
- [ ] Relevant to surrounding text
- [ ] Minimum 1200px width (desktop)
- [ ] Mobile-friendly sizes
- [ ] Caption if helpful to users

**Alt Text Examples:**
```
✅ "Porcelain tile sample showing white gloss finish with subtle gray veining"
✅ "Bathroom with large format porcelain tiles on floor and walls"
✅ "Side-by-side comparison of ceramic vs porcelain tile thickness"
❌ "tile"
❌ "image123"
❌ "click here for more info"
```

### Internal Linking
- [ ] 2-4 internal links per 1000 words
- [ ] Links to relevant cluster content
- [ ] Links to pillar pages
- [ ] Descriptive anchor text (not "click here")
- [ ] Links placed naturally in context
- [ ] Mix of exact match + branded + generic
- [ ] No follow/nofollow used sparingly

**Anchor Text Examples:**
```
✅ "Learn more about ceramic tile installation"
✅ "Complete guide to bathroom tiles"
✅ "Porcelain vs ceramic comparison"
❌ "click here"
❌ "this page"
❌ Keyword stuffing like "buy porcelain tiles dubai now"
```

### External Links
- [ ] 1-2 external links per article
- [ ] Link to authoritative sources
- [ ] Relevant to content topic
- [ ] Trusted domains only (gov, edu, established media)
- [ ] Open in new tab (_blank)
- [ ] No nofollow needed (trust the source)

### Meta Tags
- [ ] Canonical tag (self-referencing if needed)
- [ ] Robots tag set correctly (index, follow)
- [ ] Open Graph tags for social sharing
- [ ] Viewport meta for mobile
- [ ] Character encoding UTF-8

---

## Schema Markup Implementation

### Article Schema (Blog Posts)
```json
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "Page title",
  "image": ["featured-image-url"],
  "datePublished": "2024-01-15",
  "dateModified": "2024-06-15",
  "author": {
    "@type": "Person",
    "name": "Suhail Ahmed Gour"
  },
  "publisher": {
    "@type": "Organization",
    "name": "Volark Tiles",
    "logo": {
      "@type": "ImageObject",
      "url": "logo-url"
    }
  },
  "description": "Meta description text"
}
```

### Product Schema (Product Pages)
```json
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "Product Name",
  "image": ["product-images"],
  "description": "Product description",
  "brand": {
    "@type": "Brand",
    "name": "Volark"
  },
  "offers": {
    "@type": "Offer",
    "url": "product-page-url",
    "priceCurrency": "AED",
    "price": "price-range"
  },
  "aggregateRating": {
    "@type": "AggregateRating",
    "ratingValue": "4.5",
    "reviewCount": "50"
  }
}
```

### LocalBusiness Schema (Location Pages)
```json
{
  "@context": "https://schema.org",
  "@type": "LocalBusiness",
  "name": "Volark Tiles",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Maliha Road, Industrial Area 18",
    "addressLocality": "Sharjah",
    "addressCountry": "AE"
  },
  "telephone": "+971-XXXXXXXXX",
  "openingHoursSpecification": {
    "@type": "OpeningHoursSpecification",
    "dayOfWeek": ["Monday", "Tuesday"],
    "opens": "09:00",
    "closes": "18:00"
  }
}
```

### FAQ Schema (All Content with FAQ)
```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Question text?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Answer text here"
      }
    }
  ]
}
```

---

## Optimization Workflow

### Step 1: Page Audit
```
1. Review current rankings (GSC)
2. Identify primary keyword
3. Analyze top 3 competitors
4. Assess current on-page optimization
5. Note missing elements
6. Create optimization plan
```

### Step 2: Content Enhancement
```
1. Improve title/meta (if weak)
2. Enhance H1 (if vague)
3. Add missing sections
4. Strengthen introduction
5. Add visuals if needed
6. Improve CTA clarity
```

### Step 3: Technical Optimization
```
1. Fix heading hierarchy
2. Improve internal linking
3. Add/improve schema markup
4. Optimize images (alt, file names)
5. Check meta tags
6. Verify mobile rendering
```

### Step 4: Testing & Validation
```
1. Preview on mobile/desktop
2. Test links (all work?)
3. Validate schema (Schema.org)
4. Check Core Web Vitals
5. Test conversions/CTAs
6. Screen reader test (accessibility)
```

---

## Quick Win Opportunities

### High-Impact, Low-Effort Improvements

**Tier 1 (1-2 hours):**
- Improve title tag (better keyword, benefit)
- Enhance meta description (add CTA)
- Fix H1 (ensure keyword, benefit focus)
- Add internal links (2-3 to relevant pages)

**Tier 2 (2-4 hours):**
- Reorganize content (better H2/H3 structure)
- Add images/visuals (with alt text)
- Improve intro/conclusion
- Add/improve FAQ section

**Tier 3 (4-8 hours):**
- Expand content (thin content → comprehensive)
- Restructure completely (new outline)
- Add missing schema markup
- Redesign for better UX

---

## Common On-Page Issues & Fixes

| Issue | Impact | Fix | Effort |
|-------|--------|-----|--------|
| Weak title | HIGH | Rewrite with keyword + benefit | LOW |
| No H1 or multiple H1s | HIGH | Add single, clear H1 | LOW |
| Poor heading hierarchy | MEDIUM | Restructure H2/H3 levels | MEDIUM |
| Low keyword relevance | MEDIUM | Add keyword to sections | LOW |
| No internal links | MEDIUM | Add 2-4 relevant links | LOW |
| Missing schema | MEDIUM | Add Article/Product schema | MEDIUM |
| Poor mobile UX | MEDIUM | Fix layout/readability | MEDIUM |
| Thin content (< 500w) | HIGH | Expand to 1200+ words | HIGH |

---

## Seasonal Optimization

### Q4 (Oct-Dec) - Holiday Push
- Emphasize quick availability
- Highlight new collections
- Add seasonal product benefits
- Promote gift/renovation appeal

### Q1 (Jan-Mar) - New Year Resolution
- Focus on "refresh/renewal" angles
- Highlight design trends
- Promote professional installation
- Lead with transformation stories

### Q2 (Apr-Jun) - Summer Projects
- Focus on outdoor/cooling applications
- Highlight durability in heat
- Promote large format slabs
- Lead with modern designs

### Q3 (Jul-Sep) - Slower Season
- Build authority content
- Promote maintenance/care
- Create design inspiration content
- Lead with educational angles

---

## Testing & Iteration

### A/B Testing Opportunities
```
Title A: "Porcelain Tiles Dubai - Buy Now"
Title B: "Porcelain Tiles Dubai - Complete Design Guide"
(Test which gets higher CTR in Google Search)

Meta A: Short, benefit-focused
Meta B: Longer, includes CTA

H1 A: Keyword-first
H1 B: Benefit-first
```

### Metrics to Monitor
- Click-through rate (CTR) from SERP
- Average position (ranking)
- Impressions (visibility)
- Bounce rate
- Time on page
- Conversion rate
- Organic traffic growth

---

## Success Metrics

- ✅ All optimized pages rank within top 20
- ✅ Top 3 ranking improvement within 30-60 days
- ✅ CTR increases 25%+ after optimization
- ✅ Bounce rate decreases 10%+
- ✅ Time on page increases 15%+
- ✅ 90%+ of pages have proper schema markup

---

## Notes

- On-page SEO is foundation (needed but not sufficient)
- Technical SEO + Content quality + Links also matter
- Update > Optimization (fresh content ranks better)
- Mobile-first design is non-negotiable
- User experience signals now rank content
- Schema markup getting more important for visibility
