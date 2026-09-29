# Submit a Pumpkin Robot Project

The challenge uses a GSoC-style repository model:

- Your source code, build logs, and detailed documentation stay in your own repository.
- This repository stores one Markdown project profile per entry.
- You submit that profile through a pull request.
- Maintainers review the project and merge qualifying profiles into the gallery.

## What you need

Before opening a pull request, prepare:

1. A public or reviewer-accessible GitHub repository owned by you or your team.
2. A demo video showing the complete Pumpkin Robot moving and demonstrating its main interaction or AI feature.
3. A project profile based on [`PROJECT-TEMPLATE.md`](PROJECT-TEMPLATE.md).

## 1. Fork and clone this repository

Fork `D-Robotics/RDK-Community-Build` to your GitHub account, then clone your fork:

```bash
git clone https://github.com/<YOUR_USERNAME>/RDK-Community-Build.git
cd RDK-Community-Build
git remote add upstream https://github.com/D-Robotics/RDK-Community-Build.git
```

## 2. Create a branch

```bash
git switch -c showcase/<github-username>-<project-slug>
```

Keep the branch limited to one project submission.

## 3. Add your project profile

Copy the template into the challenge project directory:

```text
Pumpkin-Robot-Challenge/projects/<ParticipantName>-Project-<ProjectSlug>.md
```

Examples:

- `Maya-Project-PumpkinWalker.md`
- `TeamOrbit-Project-LanternRover.md`

Use ASCII characters in the filename. Replace every placeholder in the template and make sure the repository and video links are accessible.

## 4. Add the project to the gallery

Add one row to [`projects/README.md`](projects/README.md):

```markdown
| [Pumpkin Walker](Maya-Project-PumpkinWalker.md) | Maya | Vision + motor control | [Repository](https://github.com/...) | [Demo](https://...) |
```

Do not reorder or rewrite other entries.

## 5. Check the submission

- [ ] RDK X5 has a meaningful, documented role.
- [ ] The build has a recognizable pumpkin element.
- [ ] The finished project produces visible physical movement.
- [ ] The repository and demo links work without requesting access.
- [ ] The profile explains the architecture and how RDK X5 is used.
- [ ] The source repository includes setup instructions and a license.
- [ ] No credentials, Wi-Fi passwords, private addresses, or personal shipping information are included.

## 6. Commit and push

```bash
git add Pumpkin-Robot-Challenge/projects/
git commit -m "Add Pumpkin Robot project: <ProjectName>"
git push -u origin showcase/<github-username>-<project-slug>
```

## 7. Open the pull request

Open a pull request from your branch to `D-Robotics/RDK-Community-Build:main`.

Use this title format:

```text
[Pumpkin Robot] <Creator or Team> — <Project Name>
```

Maintainers check the project fit, profile, repository, and demo links. If changes are requested, update the same branch and push again; the pull request updates automatically.

Once approved, a maintainer merges the project profile and gallery row. Your source repository remains separate and under your control.

## What your source repository should contain

- Project overview and demo media
- Features and bill of materials
- How RDK X5 is used
- System architecture
- Setup and run instructions
- Source code
- Known limitations and safety notes
- License

Be specific in **How RDK X5 is used**: name the board, software stack, hardware interfaces, and the workloads running on the device.

## Demo video

At minimum, show:

- the complete project;
- the robot moving;
- the main interaction or AI capability;
- enough context to understand what the RDK X5 controls.

## Deadline

Open the pull request by **Oct 25**. Review changes pushed to the same pull request after the deadline may still be accepted at the maintainers' discretion.
