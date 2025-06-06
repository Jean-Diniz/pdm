# EX8-STREAM: Spark Structured Streaming

> Assignment submission format: a single ipynb file `8-stream-structured-streaming.ipynb`, as describe in step 4.
>
> Need help with Markdown? There is a quick guide [here](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

1. In this repository we have a Dockerfile for a container meant to run [Jupyter](https://jupyter.org/).
Let us inspect its content:

```bash
cat jupytercli/Dockerfile
```

This is an Alpine/Linux based image -- the Dockerfile specifies how this
container should be configured.

2. Make sure this image is build with:

```bash
make buildjupytercli
```

3. Start a container from this image -- there is a script to do this:

```bash
./jupytercli/bin/jupytercli-start.sh
```

You will be prompted with a `http` link to access the service in your browser.
Notice that the command maps directory `pdm/hostdir` into the container's path
`/app/hostdir`.

4. Follow instructions from file `/app/hostdir/8-stream-structured-streaming.ipynb`
(container's path).
