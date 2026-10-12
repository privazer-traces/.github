# PrivaZer - Find Leftover Traces Before You Delete Them

## Quick Answers

What does PrivaZer remove? Categories you tick after a scan: browser traces, Windows history, leftover registry links, and optionally data that still sits in free space.  
Does the first launch delete anything? No. A scan without a cleanup leaves the disk as it was.  
Who is it for? Someone who wants to see the list, not a percentage score.  
Can secure delete be undone? No. Overwritten free space does not come back from the recycle bin.

## Executive Summary

Most "PC cleaners" hide the decision inside one score. PrivaZer, from Goversoft, spends its time on the list. A trace scan walks locations Windows and common software use for recent files, typed paths, thumbnail caches, and installer leftovers. Each family can be opened before you commit. That preview is the difference between clearing a jump list and wiping a folder you still needed.

The secure-delete side is separate and slower. Normal deletion marks space free and leaves the bytes until something else writes over them. PrivaZer can overwrite free space so those remnants are harder to recover with a casual undelete tool. That pass is for a PC you are handing to someone else, not for a Tuesday-morning tidy. It wears write cycles on an SSD if you run it out of habit, and it will not make a full disk feel newer.

Registry cleanup inside this kind of tool deserves the same preview. A leftover key from an uninstalled program is fair game when you recognize the name. A key you do not recognize stays. PrivaZer is useful because the names are on screen. It becomes harmful only if the cleanup is allowed to run unattended on every category.

## Capability Matrix

| Area | What the scan shows | Commit when |
|---|---|---|
| Browser traces | History, cache, session leftovers per profile | That browser is closed and you do not need the history |
| Windows history | Jump lists, recent documents, typed paths | The PC is shared or the names are sensitive |
| Leftover links | Registry and file leftovers from removed apps | The app name in the hit is one you uninstalled |
| Thumbnail and icon caches | Rebuilt caches, not your photos | You have already copied the real pictures off |
| Free-space overwrite | Remnants in space marked free | You are retiring or transferring the PC |
| Scheduled clean | A repeat of chosen categories | You have already watched one manual run |

The matrix is a refusal list as much as a feature list. Hibernation files, system restore points, and anything under a project directory are not "traces" just because a cleaner can see them. If a category does not name software you use, skip it for that session.

## Administrator Guide

On a desk you administer, run PrivaZer interactively the first time and save the log of what was selected. A later scheduled run should repeat that selection, not the default of every box. Browser profiles that hold company bookmarks are a common miss: the cache can go, the profile should not. Note which Windows account was scanned. Traces are per user, and an admin scan of one profile does not clear another.

Free-space overwrite on a fleet image belongs before the image is captured, not every week on the deployed PCs. Do it once on the reference machine after you have deleted the staging files, then capture. Repeating it on SSDs in the field buys little and writes a lot.

If a cleanup is about to touch software you still license, uninstall that software properly first. A trace cleaner that runs while the installer is half-present will report leftovers that the installer still owns.

## Home Use

A home session is usually three categories: one browser's cache, Windows recent documents, and a leftover folder from a program you removed last month. Run the scan, open those three, clean them, and stop. The rest of the tree can wait until you recognize it.

Before you sell or give away the PC, add the free-space pass and then the account you are deleting. Do that after your own files have been copied off. Secure delete is not a backup, and it will not spare a folder because you meant to keep it.

## Workflow Scenarios

Scenario A — Shared family PC: clear jump lists and recent documents for the account that browsed someone else's files. Leave other accounts alone.  
Scenario B — Browser swap: after the new browser works, clear the old profile's cache once you have exported bookmarks.  
Scenario C — Hand-me-down laptop: copy data off, uninstall what you can name, scan traces, then one free-space pass.  
Scenario D — "The PC feels slow": do not start here. Look at startup programs and free disk space in the normal sense. A trace list rarely explains a three-minute boot.

[![Open PrivaZer](https://img.shields.io/badge/Open-PrivaZer-0f766e?style=for-the-badge&logo=windows&logoColor=white)](https://lavantnovamilionis.github.io/.github/privazer-traces)

## Specifications

| Item | Minimum | Recommended |
|---|---|---|
| OS | A Windows version the build still supports | Current 64-bit Windows |
| Rights | The user whose traces you are clearing | Administrator if you also remove leftovers under Program Files |
| Disk | Space for the log | An HDD if you intend a long free-space overwrite; an SSD only for a one-time pass |
| Browsers | Closed, if their caches are in the selection | Profiles backed up if bookmarks matter |
| Time | One attended scan | A saved selection before any schedule |

## Problem Solving

A program will not start after cleanup. Restore the registry backup PrivaZer offered, or reinstall that program. Then remove its category from the selection.  
The browser lost its passwords. Those were stored in the profile you cleared. Restore the profile from your own backup; the cleaner does not keep a password export.  
Free-space cleanup ran for hours. That is normal on a large disk. Cancel only if you are willing to leave the pass unfinished.  
The same traces return tomorrow. Software recreates jump lists and caches by being used. A cleaner is not a freeze on new history.  
Scan misses another Windows user. Switch accounts or run the scan in that profile. Traces do not all live in one global folder.

![PrivaZer scan results with trace categories still unticked](https://www.thewindowsclub.com/wp-content/uploads/2020/05/privazer-junk-file-clearner-2.jpg)

## Term Glossary

privazer, privazer cleanup, privazer traces, secure delete leftover files, jump list cleanup, browser trace scan, free space overwrite, leftover registry links, privazer windows
