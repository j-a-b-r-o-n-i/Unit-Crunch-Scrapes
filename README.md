# UnitCrunch Warhammer 40K Data Exports

Automatically scraped and converted faction data for [UnitCrunch](https://www.unitcrunch.com/) from Wahapedia.

## Important Disclaimer

**This data is automatically scraped and converted from Wahapedia. Errors are possible.**

- Always verify critical abilities and stats before relying on calculations
- Pattern-based conversion may miss edge cases or complex ability interactions
- Some abilities may require manual configuration in UnitCrunch
- For competitive play or maximum accuracy, consider using human-verified data packs from the [official UnitCrunch repository](https://github.com/camerongineer/UnitCrunch-data-exports)

## What's Included

Each faction has two export files:

- `{faction}-wahapedia-{date}.txt` - All units including legends
- `{faction}-wahapedia-no-legends-{date}.txt` - Standard units only

Files are in MessagePack format compatible with UnitCrunch v0.73+.

## How to Use

### Import into UnitCrunch

1. Download the `.txt` file for your desired faction
2. Go to [UnitCrunch](https://www.unitcrunch.com/)
3. Click "Import Data"
4. Select the downloaded file
5. Review and verify the imported data

### Verify Your Data

After importing, check:

- Critical abilities are present and correctly configured
- Weapon stats match your codex
- Special rules and conditions are accurate
- Unit points costs are current

## Known Limitations

### Pattern Detection

The conversion uses pattern matching to detect abilities. This means:

- Complex conditional abilities may be simplified
- Phase-specific restrictions may be omitted (toggle abilities as needed)
- Faction-specific mechanics may require manual addition
- Stratagem-like effects are not included

### Ability Coverage

While many common patterns are detected, some abilities may be missing or incomplete:

- Multi-condition triggers
- Complex aura effects
- Abilities with variable effects based on game state
- Some faction-specific special rules

### Recommendations

- Use these exports as a starting point
- Manually verify abilities for units you use frequently
- For tournament preparation, cross-reference with official human-verified packs
- Report significant errors or missing patterns to help improve future exports

## Data Sources

- **Source Data**: [Wahapedia](https://wahapedia.ru/wh40k10ed/factions/)
- **Target Format**: [UnitCrunch](https://www.unitcrunch.com/)

## Alternative Data Packs

For human-verified, tournament-ready data:

- [UnitCrunch Official Data Exports](https://github.com/camerongineer/UnitCrunch-data-exports) - Community-maintained, verified exports
- [Icon Bearer Packs](https://github.com/camerongineer/UnitCrunch-data-exports) - High-quality faction data

## Updates

These exports are generated periodically from Wahapedia. Check the date in the filename to see when data was last updated.

## License

This is unofficial fan-made content. Warhammer 40,000 is a trademark of Games Workshop Ltd. Data sourced from Wahapedia under fair use for personal tabletop gaming purposes.

## Feedback

Found an error or missing ability? While this data is automatically generated, feedback helps improve the pattern detection for future exports.
