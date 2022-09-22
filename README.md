# tranquility

## For Windows Users

Install WSL
`https://learn.microsoft.com/en-us/windows/wsl/install`

Within WSL Terminal Run:

```bash
sudo apt-get update 
sudo apt-get upgrade 
sudo apt-get install make flex bison
```

## Build

Within Tranquility Directory & WSL Terminal Run:

```bash
make
```

Returns `tranqc`

## Usage

Create `main.t`
*Use `touch main.t` while in tranqulity directory*

Create `index.html`
*Use `touch index.html` while in tranqulity directory*

Insert code into `main.t` and save, manual starts with these lines:
```
fun init() {
    sprint("Hello World\n")
}
```

Insert code into `index.html` and save, you can use this as a template:
```html
<html>
<head>
<script src="main.json"></script>
<script src="https://www.cs.drexel.edu/~bls96/tvm.js"></script>
</head>
<body>
</body>
</html>

```

Within Tranquility Directory & WSL Terminal Run:
```bash
./tranqc main.t
```

Returns `main.json`

Open `index.html` in browser

## Credit

Brian L. Stuart <blstuart@drexel.edu>
