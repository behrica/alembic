# 0.2.0

- Add load-project, and make distill print changes
  The load-project function will read the current project.clj file's 
  dependencies and load any new ones.

  The distill function now prints the dependency coordinates that are 
  loaded, and separately those that are not due to conflicts.  It also now
  accepts a sequence of dependencies to load.

  The previous return behaviour of distill is available in distill*.

# 0.1.4

- Update to classlojure 0.7.0
  Removes transitive dependency on useful.

# 0.1.3

- Don't read project.clj when :repositories passed to distill

# 0.1.2

- Allow disabling version mismatch messages at the console.

  They can be turned off by passing `false` to the option `:verbose?` in
  `distill` and `add-dependency`.

- Add no-arg arity to `project-dependencies`

  Describes the :repositories option for distill in the readme, mentioning
  project-dependencies.


# 0.1.1

- Add clojure 1.4 dependency

- Normalise :repositories to be a map

# 0.1.0

- Initial version
