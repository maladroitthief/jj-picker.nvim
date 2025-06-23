# jj-picker.nvim

A jj status picker to be used with folke's [snacks](https://github.com/folke/snacks.nvim)

## Usage

```lua
return {
	"folke/snacks.nvim",
	dependencies = {
		"maladroitthief/jj-picker.nvim",
  },
	priority = 1000,
	lazy = false,
	keys = {
		{
			"<leader>js",
			function()
				require("jj-picker").status()
			end,
			mode = { "n" },
			desc = "snacks: jj status",
		},
  },
}
```
