data('ToothGrowth')
View(ToothGrowth)

# filter
filtered_tg <- filter(ToothGrowth, dose == 0.5)
View(filtered_tg)

# sort
arrange(filtered_tg, len)

arrange(filter(ToothGrowth, dose == 0.5), len)

# use pipe
filter_toothgrowth <- ToothGrowth %>%
  filter(dose==0.5) %>% 
  group_by(supp) %>% 
  summarize(mean_len = mean(len,na.rm=T),.group="drop")
