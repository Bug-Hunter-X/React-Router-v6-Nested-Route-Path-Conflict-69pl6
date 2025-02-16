# React Router v6 Nested Route Path Conflict

This repository demonstrates a potential issue in React Router v6 when dealing with nested routes that have overlapping path segments.  The problem arises when a nested route's path is a more specific version of its parent's path, leading to unexpected rendering or routing errors.

## Problem

The `bug.js` file contains a React Router setup with nested routes. The `/about` route and the `/about/nested` route lead to a conflict. When navigating to `/about/nested`, the routing logic might behave unexpectedly or fail to render the `NestedAbout` component correctly.

## Solution

The `bugSolution.js` file provides a solution using more precise path matching. By changing the `path` property in routes, we can avoid such path conflicts and ensure correct routing behavior.

## Setup

1.  Clone this repository.
2.  Navigate to the project directory.
3.  Run `npm install` to install dependencies.
4.  Run `npm start` to start the development server.