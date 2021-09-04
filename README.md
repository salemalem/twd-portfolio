[![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://github.com/kt3k/twd)


# twd-portfolio
Personal portfolio at shyngys.mod.land powered by Tailwind CSS

## Install <a href="https://github.com/kt3k/twd">twd</a>
```cmd
deno install --allow-read=. --allow-write=. --allow-net=deno.land,esm.sh,cdn.esm.sh -fq https://deno.land/x/twd@v0.4.8/cli.ts
```

## index.html
write tailwind components with classes as it's written in this repo.

Link css to tailwind.css or name as you want with .css
This css will be used to output tailwind.
Because Tailwind doesn't download all css, rather downloads only used classes each time due to large file size, we need to write the following command to extract cdn tailwind to styles.css
```
twd -w ./index.html -o ./tailwind.css
Output: 
Using default settings. You can optionally configure it by 'twd.ts' config file.
Writing styles to file 'tailwind.css'
Builtin 89ms
```

-w flag is used to watch file changes instead of reexecuting the command each time.
