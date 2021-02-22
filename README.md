# PR check list

- [ ] White spaces, formating
- [ ] Use of #region
- [ ] Using is sorted and unused references are removed
- [ ] Naming conventions
   * Singular and Plurals
   * Filename matches class name
- [ ] Resharper
- [ ] Localization
   * FoH: Enums are not localized
   * API: Dto exists for Enums and is used in Automapper
- [ ] Think about the overall design
   * Does the fix only batch the symptoms or the real cause?

# Merge check list

- [ ] Is the migration number correct?
   * Does the migration run (locally)?
- [ ] Does it build
   * Check pipeline build for PR
   * API: manually trigger a branch build (until we can figure out why the automatic build doesn't work anymore)
- [ ] Do the unit tests run and succeed?
- [ ] Will it affect other components (FOH, BOH, API, HUB)?
   - Hold of merge when other PRs are not yet approved.
