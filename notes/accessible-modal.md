# Accessible Modal Dialogs

## Focus management
- Move focus into dialog on open (focus first focusable or dialog itself).
- Trap focus within dialog while open.
- Return focus to trigger element on close.

## Keyboard support
- `Esc` closes dialog.
- `Tab` / `Shift+Tab` cycles within dialog.
- Don't let focus escape to background.

## ARIA
- `role="dialog"` and `aria-modal="true"`.
- `aria-labelledby` points to visible title.
- Optionally `aria-describedby` for description.

## Testing
- Check with NVDA and VoiceOver.
- Verify focus order with keyboard only.
- Ensure background is inert or hidden from AT.
