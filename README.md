# Bachelorarbeit

Dieses repo ist das LaTeX template für die Bachelorarbeit der Westfälischen Hochschule, für den Fachbereich Informatik.

Dies ist ein Klon des [Overleaf templates von Nico Hülscher][1] (veröf. 17. Juli 2023).

# Nutzung

1. erfordert, dass LaTeX installiert ist
2. den LaTeX- oder anderen Texteditor mit LaTeX-Erweiterung (bspw. [VimTeX][2] für Vim und NeoVim)
3. Unbedingt kompilieren mit "LuaLaTeX + MakeIndex + BibTeX"
3.1 TeXworks editor: "LuaLaTeX + MakeIndex + BibTeX"
3.2 VimTex NeoVim Beispielconfig (lua):
```lua
return {
	"lervag/vimtex",
		lazy = false,
			init = function()
			vim.g.vimtex_view_method = "general"
			vim.g.vimtex_view_general_viewer = "masterpdfeditor"
			vim.g.vimtex_compiler_latexmk_engines = {
				["_"] = "-lualatex",
			}
			end
}
```

# Lizenz

Die originale Lizenz wird hier beibehalten. Sollte sich das offizielle Design/Format der WHS für Informatik ändern,
sind pull requests mit entsprechenden Änderungen willkommen.



  [1]https://www.overleaf.com/latex/templates/vorlage-bachelorarbeit-informatik-westfalische-hochschule/ympzbtzjqhdd
  [2]https://github.com/lervag/vimtex
