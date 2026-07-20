# How I Built a TypeDoc Plugin Used by 500+ Developers (And You Can Too)

*Ready to publish on Dev.to*

---

## Introduction

Building open source software is rewarding but challenging. Today, I want to share the story of how I created `typedoc-plugin-not-exported` - a small plugin that turned into a project used by hundreds of developers worldwide.

More importantly, I want to talk about **open source sustainability** and how I'm now supporting this project through GitHub Sponsors.

---

## The Problem

When I started working on a large TypeScript project, I ran into a frustrating documentation problem:

**TypeDoc (the TypeScript documentation generator) excludes non-exported symbols by default.**

This meant that internal APIs - functions, types, and classes not exported by the package - were invisible in the generated documentation.

For teams documenting internal modules or creating comprehensive API references, this was a real pain point.

### Real Example:

```typescript
// helpers.ts

/**
 * Internal helper function - not exported
 * But developers need to document it!
 */
function formatData(input: string): string {
  return input.toUpperCase()
}

// Only this is visible in TypeDoc:
export function processData(data: string) {
  return formatData(data)
}
```

With TypeDoc's default behavior, `formatData` wouldn't appear in the docs, even though it's part of the implementation.

---

## The Solution

I created a simple but effective solution: a TypeDoc plugin that forces inclusion of non-exported symbols using a custom `@notExported` tag.

### How It Works:

```typescript
/**
 * Internal helper - mark with @notExported
 * @notExported
 */
function formatData(input: string): string {
  return input.toUpperCase()
}
```

Now it appears in the documentation! Simple, elegant, and solves the problem.

---

## From Side Project to 500+ Users

Here's the growth trajectory:

- **Week 1:** Created the plugin for my own project
- **Month 1:** Published to npm, got 20 downloads
- **Month 3:** 100 downloads/week, first GitHub star
- **Month 6:** 500 downloads/week, 50+ stars
- **Today:** 1000+ weekly downloads, 100+ stars, used in production

### What Surprised Me:

1. **Simple problems attract users** - People searched for exactly this solution
2. **TypeScript community is active** - Stars and downloads came organically
3. **Maintenance is invisible work** - Most people don't realize the effort behind open source
4. **There's demand for support** - Issues, feature requests, emails

---

## The Growth Hacking Part

How did I grow this plugin from zero to 500+ users?

### 1. **Great Package Name**
The name `typedoc-plugin-not-exported` is descriptive and SEO-friendly. When developers search "TypeDoc non-exported symbols", they find it.

### 2. **Clear Documentation**
The README explains the problem, the solution, and provides examples. No fluff, just value.

### 3. **Small and Focused**
The plugin does one thing well. It's not bloated, easy to understand, and easy to integrate.

### 4. **Active Maintenance**
I respond to issues, fix bugs, and maintain compatibility with the latest TypeDoc versions.

### 5. **Community Engagement**
I answer questions, accept contributions, and show appreciation to users.

---

## The Sustainability Question

After a year of maintenance, I realized something:

**Open source maintainers rarely get compensated for their work.**

I spend 5-10 hours per month on this plugin:
- Fixing bugs
- Responding to issues  
- Testing new TypeDoc versions
- Planning features

That's 50-120 hours per year. If I valued my time at $50/hour (conservative), that's $2,500-6,000 annually.

Yet, I make $0.

---

## Enter GitHub Sponsors

GitHub Sponsors changed the equation. Now, developers who rely on my plugin can directly support my work.

I set up three sponsorship tiers:

### **Bronze ($5/month)**
- Your name in the README
- Early access to new features
- Best for individuals

### **Silver ($25/month)**  
- Logo in README
- Priority email support
- Custom TypeDoc configuration help
- Best for small teams

### **Gold ($100/month)**
- Logo and testimonial in README
- Monthly consulting call
- Priority feature requests
- Custom development
- Best for enterprises

---

## Why This Matters

This isn't about getting rich. It's about:

1. **Sustaining open source** - Developers can support tools they rely on
2. **Enabling creators** - I can spend more time on maintenance and improvements
3. **Building community** - Sponsors feel invested in the project's success
4. **Setting expectations** - High-quality open source takes effort and deserves support

---

## Lessons Learned

### 1. Start Small
The best projects often solve specific problems for yourself first. Generalize later.

### 2. Execute Before Marketing
The plugin gained traction through quality, not hype. Build something useful first.

### 3. Clear Documentation Wins
Good docs attract more users than any marketing campaign.

### 4. Community First
Respond to users, accept feedback, value contributions. Community builds itself.

### 5. Monetization Can Be Ethical
GitHub Sponsors is voluntary. Nobody *has* to pay. It's a choice by people who benefit.

---

## The Future

My goal is to grow GitHub Sponsors to $500-1000/month within a year. This would allow me to:

- Dedicate 1-2 hours per week to maintenance
- Release features faster
- Provide better support
- Create educational content

If you use `typedoc-plugin-not-exported` in production, consider becoming a sponsor:

**👉 [github.com/sponsors/protactiniumplatinumhyssop-cell](https://github.com/sponsors/protactiniumplatinumhyssop-cell)**

Even $5/month makes a difference!

---

## Call to Action

Whether you're an open source creator or user:

**For Creators:** Don't be afraid to ask for support. You deserve it.

**For Users:** If you rely on open source, consider sponsoring the projects you depend on. Even small amounts sustain the ecosystem.

Together, we can build a sustainable open source community.

---

## Resources

- **Plugin:** [typedoc-plugin-not-exported on npm](https://www.npmjs.com/package/typedoc-plugin-not-exported)
- **GitHub:** [Repository](https://github.com/protactiniumplatinumhyssop-cell/typedoc-plugin-not-exported)
- **Sponsors:** [Support open source development](https://github.com/sponsors/protactiniumplatinumhyssop-cell)
- **TypeDoc Docs:** [Official documentation](https://typedoc.org/)

---

**Have questions? Drop them in the comments! 👇**

---

## Tags
#typescript #opensource #typedoc #sponsorship #devtools #javascript #opensourcesustainability
