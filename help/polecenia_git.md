# Polecenia Git

## Status, dodawanie i zatwierdzanie zmian
“%s”
Sprawdź stan swojego repozytorium, aby dowiedzieć się, czy nastąpiły zmiany. Uruchom terminal skrótem Ctrl-` . Terminal uruchomi się w katalogu (obszarze roboczym), który masz otwarty w VSC

* Sprawdź, czy są wymienione zmiany: `git status`. Otrzymasz podobny komunikat

     >On branch main
     >*Na głównej gałęzi*
     >
     >Your branch is up to date with 'origin/main'.\
     >*Twoja gałąź to 'origin/main*.
     >
     >Changes to be committed:\
     >*Zmiany, które należy zatwierdzić*
     >>(use "`it restore --staged <file>...` to unstage)\
     >>*(użyj `git restore --staged <file>...`, aby [przywrócić pliki](https://stackoverflow.com/questions/58003030/what-is-the-git-restore-command-and-what-is-the-difference-between-git-restor).\
     >>>new file:   pl-PL_kickstart_7.1.2_lang/pl-PL.kickstart.ini
     >>>nowy plik:  pl-PL_kickstart_7.1.2_lang/pl-PL.kickstart.ini
     >
     >Changes not staged for commit:\
     >*Zmiany nie zostały przygotowane do zatwierdzenia:*
     >>(use `git add <file>...` to update what will be committed)\
     >>*(użyj `git add <file>...`, aby zaktualizować to, co zostanie wysłane)*
     >>
     >>(use `git restore <file>...` to discard changes in working directory)\
     >>*(użyj `git restore <file>...`, aby odrzucić zmiany w katalogu roboczym)*
     >>
     >>>modified:   LICENSE\
     >>>*(zmodyfikowane:) Lista zmodyfikowanych plików np.:*
     >>>>modified: LICENSE\
     >>>>modified: .gitignore
     >
     >Untracked files:\
     >*Pliki nieśledzone:*\
     >>(use `git add <file>...` to include in what will be committed)\
     >>*(użyj polecenia `git add <file>...`, aby dołączyć do tego, co zostanie    wysłane)*\
     >>>*lista nieśledzonych plików np:*\
     >>>>.gitignore\
     >>>>pl-PL_kickstart_7.1.2_lang/
     >
     >no changes added to commit (use `git add` and/or `git commit -a`)\
     >(brak zmian dodanych do commitu (użyj `git add` i/lub `git commit -a`)

* Wybierz , które z nieśledzonych plików chcesz dodać do zatwierdzenia śledzenia (czyli zapisać) np.:
  >`git add pl-PL_kickstart_7.1.2_lang` dla pojedyńczych plików lub\
  >`git add --all` dla wszystkich plików\

* Zatwierdź zmiany śledzonych plików (commit)
  >`git commit -a` - dla wszystkich zmienionych plików
  >`git commit -m "<your commit message>"` z krótkim opisem aktualizacji.

1. git add `[<options>] [--] <pathspec>...`

    -n, --dry-run         dry run
    -v, --verbose         be verbose

    -i, --interactive     interactive picking
    -p, --patch           select hunks interactively
    -e, --edit            edit current diff and apply
    -f, --force           allow adding otherwise ignored files
    -u, --update          update tracked files
    --renormalize         renormalize EOL of tracked files (implies -u)
    -N, --intent-to-add   record only the fact that the path will be added later
    -A, --all             add changes from all tracked and untracked files
    --ignore-removal      ignore paths removed in the working tree (same as --no-all)
    --refresh             don't add, only refresh the index
    --ignore-errors       just skip files which cannot be added because of errors
    --ignore-missing      check if - even missing - files are ignored in dry run
    --sparse              allow updating entries outside of the sparse-checkout cone
    --chmod (+|-)x        override the executable bit of the listed files
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

1. git commit [<options>] [--] <pathspec>...

    -q, --quiet           suppress summary after successful commit
    -v, --verbose         show diff in commit message template

Commit message options
    -F, --file <file>     read message from file
    --author <author>     override author for commit
    --date <date>         override date for commit
    -m, --message <message>
                          commit message
    -c, --reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --reuse-message <commit>
                          reuse message from specified commit
    --fixup [(amend|reword):]commit
                          use autosquash formatted message to fixup or amend/reword specified commit
    --squash <commit>     use autosquash formatted message to squash specified commit
    --reset-author        the commit is authored by me now (used with -C/-c/--amend)
    --trailer <trailer>   add custom trailer(s)
    -s, --signoff         add a Signed-off-by trailer
    -t, --template <file>
                          use specified template file
    -e, --edit            force edit of commit
    --cleanup <mode>      how to strip spaces and #comments from message
    --status              include status in commit message template
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --all             commit all changed files
    -i, --include         add specified files to index for commit
    --interactive         interactively add files
    -p, --patch           interactively add changes
    -o, --only            commit only specified files
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --dry-run             show what would be committed
    --short               show status concisely
    --branch              show branch information
    --ahead-behind        compute full ahead/behind values
    --porcelain           machine-readable output
    --long                show status in long format (default)
    -z, --null            terminate entries with NUL
    --amend               amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    -u, --untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character
