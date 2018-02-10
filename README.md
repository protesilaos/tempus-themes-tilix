# Tempus themes for Tilix terminal

## Automatic installation

If you use Arch Linux or derivatives, you can get these themes from the [AUR](https://aur.archlinux.org/packages/tempus-themes-tilix/).

## Manual installation instructions

The theme files can be located in either of two places:

- At `/usr/share/tilix/schemes/` which makes them accessible to all users (requires root privileges).
- Or `~/.config/tilix/schemes/` for use by the current user (directory path needs to be created if it does not already exist).

Choose whatever option suits your needs. The following document will use the latter as a working example.

### We use the command line

Start by cloning the `tempus-themes-tilix` repo and entering it (unless you prefer copy-pasting, in which case you need to get the files manually and adapt accordingly):

```sh
git clone https://github.com/protesilaos/tempus-themes-tilix.git --depth 1 && cd tempus-themes-tilix
```

### Prepare the destination directory

*This step is normally not needed if you copy the files to `/usr/share/tilix/schemes/`.*

Then make sure you have the local directory to store the files. Run the following command, excluding the lines that start with `#` (those are comments):

```sh
# Create directory if it does not already exist
mkdir -p ~/.config/tilix/schemes/
```

### Copying the theme file

Now just copy the file you wish to use. The following command will have `tempus_winter` as an example:

```sh
cp tempus_winter.json ~/.config/tilix/schemes/
```

Done.

The theme will then be available from the application's preferences window, in the profiles' section (under the colours tab).

### Copying all themes

You want to test them all out? A simple command to copy everything:

```sh
cp *.json ~/.config/tilix/schemes/
```

Enjoy!

## Additional resources

For all available ports, refer to the main [Tempus themes repo](https://github.com/protesilaos/tempus-themes).

## Contributing

All contributions should be submitted to the Tempus themes generator. See [CONTRIBUTING.md](https://github.com/protesilaos/tempus-themes-generator/blob/master/CONTRIBUTING.md).

## License

GNU General Public License Version 3. See [LICENSE](https://github.com/protesilaos/tempus-themes-tilix/blob/master/LICENSE).
