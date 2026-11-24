# Deadline notice checks

This note records the checks run on this branch.

## Pass

The fixed code was built with two jobs.
The deadline notice filter passed 17 tests.
The budget boundary filter passed 8 tests.

The order test passed.
A past deadline with an open call puts the tool result next.
The open call test passed.
A due notice waits until that call is answered.
The budget test passed.
An 840 second turn still warns at the first rung.
The near deadline test passed.
A turn with no open call still gets the notice.

## Guard removed

The early return was taken out.
The same four tests were built again.
The order test failed.
The messages were assistant, then user, then tool.
The user text starts with the time marker.
The open call test failed.
The notice was added while the call was still open.
The budget test passed.
A quiet first reading still stores the whole budget.
The near deadline test passed.
A turn with no open call stayed the same.

## Scope

The full crate suite was not run.
The full workspace suite was not run.
These checks cover the two files this branch edits.
