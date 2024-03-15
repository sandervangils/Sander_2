# Sander_2
remotes::install_github('jaburgoyne/compmus')


wood <-
  get_tidy_audio_analysis("6IQILcYkN2S2eSu5IHoPEH") |>
  select(segments) |>
  unnest(segments) |>
  select(start, duration, pitches)
  