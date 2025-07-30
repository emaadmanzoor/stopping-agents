# Stopping Agents Demo App
<img src="https://stoppingagents.com/images/logo-transparent.png" height="150" align="right"/>

> [!WARNING]  
> This is work-in-progress, largely vibe-coded with [Codex CLI](https://github.com/openai/codex), and not performant.

We built a [Rich](https://github.com/Textualize/rich)/[Textual](https://github.com/textualize/textual/) TUI app to showcase stopping agents that optimally stop sales conversations. To try this out, simply run the commands below in this directory:

```bash
./stoppingagents --audio-file [PATH TO A RECORDED SALES CALL .WAV] [--gpu]
```

The `datasets` folder has an `example_sales_call.wav` extracted from
[this video](https://www.youtube.com/watch?v=Ms5zYSwoqOs) to test with.

## TODO

- [ ] Add listening to a live audio stream
- [ ] Find and fix performance issues
- [ ] Fix responsivity to terminal size
- [ ] Make deployable and installable
- [ ] Document installation and usage
- [ ] Add more user configuration options
