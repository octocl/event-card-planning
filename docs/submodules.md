# Working with EventCard submodules

The planning repository links two independent Git repositories: [backend](https://github.com/octocl/event-card-backend) at `backend/` and [frontend](https://github.com/octocl/event-card-frontend) at `frontend/`. `.gitmodules` stores their URLs; the planning repository stores the exact commit selected from each. Code changes belong in the child repository, while updating the selected commit belongs in planning.

## Clone everything

```sh
git clone --recurse-submodules https://github.com/octocl/event-card-planning.git
```

If planning was already cloned without its submodules, run `git submodule update --init --recursive` inside it.

## Make a future backend or frontend change

1. Enter `backend/` or `frontend/`, then run `git switch main`. A fresh submodule clone may start at a detached commit.
2. Make the change, commit it in that repository, and push its `main` branch.
3. Return to the planning repository. Run `git add backend` or `git add frontend`, commit that pointer change, and push planning.

The child commit must be pushed before the planning pointer; otherwise other people cannot fetch the commit planning references. To inspect the recorded versions, run `git submodule status` from the planning repository. No implementation work is planned yet.
