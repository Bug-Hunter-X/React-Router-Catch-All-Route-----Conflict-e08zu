# React Router Catch-All Route Conflict

This repository demonstrates a common issue in React Router v6 where a catch-all route (`*`) placed before more specific routes causes unexpected behavior.  The `*` route will match *any* path, effectively preventing other routes from ever being accessed.

## Problem

The problem arises when the `*` route is declared before other routes.  This is because React Router evaluates routes in order, and the catch-all route will always match, thus overshadowing other routes.