# Draggin' Wagons Towing - Website v1

Static HTML/CSS/JS site. No build step, no framework - open any `.html` file directly in a browser, or serve the folder with any static host.

## Structure
- `index.html` - Home
- `services.html` - Full service breakdown
- `service-area.html` - Bryan County OK & Marshall County OK coverage
- `about.html` - Father & son team bios
- `contact.html` - Contact info, hours, map
- `css/style.css` - All styles (brand colors as CSS variables at the top)
- `js/main.js` - Mobile nav toggle only, no scroll animations
- `images/` - Real photos pulled from the owner's files (logo, truck, crew, job photos)

## Images currently in use
- `draggin-wagons-logo.jpg` / `favicon.jpg` - real logo, from the owner's Facebook photo
- `hero-truck.jpg` - real flatbed parked at the Durant shop
- `team-father-son.jpg` - real crew photo on one of the wreckers (shows 3 people, so it's used as a general crew shot rather than labeled as specifically father & son)
- `gallery-1.jpg` - real photo, SUV loaded on the flatbed
- `gallery-2.jpg` - real photo, night tow outside Arby's

## TODO before launch
1. **Individual headshots**: if you want real headshots next to each bio (instead of just the shared crew photo), send two individual photos and I'll drop them in.
2. **Reviews**: the 3 testimonials on the homepage are written as realistic samples, not pulled from actual Google reviews (the Maps page is JS-heavy and didn't return review text). Swap in real quotes, and update the `reviewCount` in the JSON-LD schema in `index.html` once you confirm the real number of Google reviews.
3. **Domain/canonical URLs**: all pages assume `https://www.dragginwagonstowing.com/`, update `robots.txt`, `sitemap.xml`, and the `<link rel="canonical">` / `og:url` tags if the final domain differs.

## Ownership note
Owned/operated by Russ Parker and Shane Parker (father & son co-owners), with a third silent partner who is a veteran and asked not to be named on the site. That silent partner's service is why the site says "veteran owned" without naming him.

## SEO notes
- Each page has unique title/meta description targeting SE Oklahoma towing keywords (Durant, Madill, Bryan County, Marshall County).
- Company only tows in Oklahoma (Bryan & Marshall County) - no Texas cities/counties are named anywhere on the site, per the owner's licensing constraints.
- `images/ok-service-area-map.svg` - Oklahoma county map (county shapes from the public-domain Wikimedia/Benbennick county-highlight series) with Bryan & Marshall County recolored in brand green. Used on the homepage and service-area page.
- `TowingService` JSON-LD schema on the homepage for local business rich results.
- `robots.txt` + `sitemap.xml` included.
- Semantic heading structure (one `<h1>` per page).

## Style notes
- No em dashes anywhere in the copy, by request.
- White background throughout, minimal hairline-bordered cards instead of shadows/color blocks, one accent color (green) used sparingly.
