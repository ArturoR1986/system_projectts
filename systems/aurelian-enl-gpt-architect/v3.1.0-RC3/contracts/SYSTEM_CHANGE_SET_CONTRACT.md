# SYSTEM_CHANGE_SET_CONTRACT

Version: 1.0-RC1

## Purpose

Defines one atomic architecture update so ENL can eventually apply system-project changes through Git/source-control workflows instead of manual copy/paste reconciliation.

## Required Fields

```yaml
change_id:
target_system:
base_version:
candidate_version:
change_type: patch | minor | architecture
reason:

files_added: []
files_modified: []
files_superseded: []

router_impact:
manifest_impact:
command_impact:
registry_impact:
memory_impact:
skill_impact:
governance_impact:

tests_added_or_updated: []
migration_steps: []
rollback_steps: []

authority:
  prepared_by:
  reviewed_by:
  approval_required:

state: PROPOSED | PREPARED | COMMITTED | PULL_REQUEST_OPEN | APPROVED | MERGED | DEPLOYED | VERIFIED | ROLLED_BACK
```

## Rules

- One Change Set describes one coherent behavior change.
- Manifest changes are mandatory when active inventory/status/path changes.
- Router changes are mandatory when activation/routing changes.
- Tests are mandatory for behavior changes.
- State labels represent actual external state, not intention.
- Human approval remains visible for consequential promotion/release.
- A failed Change Set must have a rollback path.

## Future Automation Target

```text
ENL design/change
→ Change Set
→ branch
→ patch files
→ reconcile manifest/router/registries
→ run tests
→ diff
→ human review
→ merge
→ deployment mirror/runtime update
→ verification
```
