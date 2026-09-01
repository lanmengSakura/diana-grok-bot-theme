# Diana Grok Bot Theme 0.1.0-rc.1

Status: **source pre-release; visual blueprint only**.

## Public implementation

- Publishes reviewable CSS, local artwork, placeholder mapping, documentation, and validation.
- Publishes no executable adapter, debugging launch command, listener, process state, local path, screenshot, or target binary.
- The repository alone does not claim a live mount.

## Compatibility snapshot

- Full artwork was last verified on Grok Bot `0.28.0`.
- Day/night mode, the bottom-layer black-hole ornament, responsive artwork, and interaction pass-through were visually checked in that build.
- A newer build requires a fresh renderer/selector audit.

## Final release gate

- Re-run the private adapter against a clean Grok Bot `0.28.0` launch.
- Verify day/night, black-hole stacking, input area, long conversation, narrow/maximized layout, restart, and restore.
- Confirm every decorative node remains below controls and ignores pointer input.
- Run `npm test`, record target executable signature, and inspect the public repository tree once more.
