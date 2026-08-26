# Accessibility Audit Checklist

Quick reference for manual audits.

## Keyboard

- [ ] All interactive elements reachable via Tab in logical order
- [ ] Focus visible: `:focus-visible` styles not removed
- [ ] No keyboard traps; escape closes dialogs/menus
- [ ] Skip link present and visible on focus

## Semantics

- [ ] Landmarks: header, nav, main, footer
- [ ] Heading levels do not skip
- [ ] Buttons vs links used correctly
- [ ] Form inputs have associated `<label>`

## ARIA

- [ ] ARIA only when native HTML is insufficient
- [ ] `aria-expanded` toggles correctly on disclosure widgets
- [ ] Dialog uses `role="dialog"` and `aria-modal` where appropriate
- [ ] Live regions for dynamic updates (`aria-live="polite"`)

## Colour & Contrast

- [ ] Text contrast ≥ 4.5:1 (3:1 for large text)
- [ ] Meaning does not rely on colour alone
- [ ] Focus indicators have contrast against adjacent colours

## Images & Media

- [ ] Informative images have `alt` text
- [ ] Decorative images use `alt=""`
- [ ] Video has captions and audio descriptions where needed

## Motion

- [ ] No flashing > 3 times/second
- [ ] Animations respect `prefers-reduced-motion`

## Mobile / Touch

- [ ] Target size at least 44×44 px
- [ ] Horizontal scroll avoided at 320px width

## Testing Tools

- axe DevTools / Lighthouse
- WAVE
- Keyboard-only navigation
- VoiceOver / NVDA / TalkBack
