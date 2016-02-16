# zen-of-data-processing

1. separate initial data processing of data types (string vs date etc) from other manipulation tasks
2. save the data with proper types as a binary represenation (eg .rds) to be pulled in from all subsequent files
3. ** Given a destructive change, a new object should be created **
  * `new_df <- df %>% mutate(some_col = some_irreversible_change(some_col))`
