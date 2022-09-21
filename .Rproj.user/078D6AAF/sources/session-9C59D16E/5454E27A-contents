
mutate(state_moderate = case_when(
  state %in% c("Bago (West)", "Bago (East)") ~ 1133432, 
  state %in% c("Shan (North)", 
               "Shan (East)", 
               "Shan (South)") ~ 203729, 
  TRUE ~ state_moderate), 
  state_severe = case_when(
    state %in% c("Bago (West)", "Bago (East)") ~ 267769, 
    state %in% c("Shan (North)", 
                 "Shan (East)", 
                 "Shan (South)") ~ 94328, 
    TRUE ~ state_severe))


summarise(state_insecure = max(state_insecure), 
          tsp_pin = sum(tsp_pin), 
          state_severe = max(state_severe), 
          tsp_severe = sum(tsp_severe), 
          state_moderate = max(state_moderate), 
          tsp_moderate = sum(tsp_moderate))