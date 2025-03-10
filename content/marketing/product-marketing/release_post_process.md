# Release post process

Product marketing is responsible for creating the monthly release post in collaboration with the product and content teams. Here is an overview of the process:

**10 days before release ships**

- Product marketing generates the release post template with placeholder section for highlights

**7 days before release ships**

- PMs to recommend which updates to feature and provide draft copy and assets (videos, links, screenshots) for all highlights directly to the PR.
- If assets aren't ready, PM to add a placeholder for expected assets.

**Within 24 hours after the release is cut**

- VP Product runs the script to generate changelog and merges it into the release template
  - Note: make sure to update the _version number_ in the script itself. If for some reason the version number isn't added yet and you need to capture the "Unreleased" then passing it the literal string match for the "Unreleased" heading, usually `Unreleased`, in place of a version number works)

```
# in the root dir of the aourcegraph/about repo, make sure the latest sourcegraph/sourcegraph repo
# CHANGELOG.md file is at ../sourcegraph/CHANGELOG.md, then run:
go run ./bin/generate_changelog_items.go -versions 3.28 -i ../sourcegraph/CHANGELOG.md
```

- If necessary, PMs make edits to the changelog based on what was actually shipped.
- PMs add final assets.
- Product marketing to package and draft the release post and share with Rebecca, Andy, and Christina for review.

**0-2 days after release ships**

- No new additions or edits from the product team
- Managing Editor edits and publishes release post.
