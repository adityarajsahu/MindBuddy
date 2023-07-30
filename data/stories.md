## happy path
* greet
  - utter_greet
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## ask mental health
* ask_mental_health
  - utter_mental_health

## ask anxiety signs
* ask_anxiety_signs
  - utter_anxiety_signs

## ask cure depression
* ask_cure_depression
  - utter_cure_depression

## ask mindfulness
* ask_mindfulness
  - utter_mindfulness

## ask mood swings
* ask_mood_swings
  - utter_mood_swings

## ask sleep
* ask_sleep
  - utter_sleep

## ask seek therapy 
* ask_seek_therapy
  - utter_seek_therapy

## ask exercise
* ask_exercise
  - utter_exercise

## ask self care
* ask_self_care
  - utter_self_care

## ask reduce stigma
* ask_reduce_stigma
  - utter_reduce_stigma

## ask lower stress
* ask_lower_stress
  - utter_lower_stress

## ask eat healthy
* ask_eat_healthy
  - utter_eat_healthy

## ask exercise amount
* ask_exercise_amount
  - utter_exercise_amount

## survey happy path
* greet 
  - utter_greet
* affirm
  - health_form
  - form{"name":"health_form"}
  - form{"name":null}
  - utter_slots_values
* thankyou
  - utter_no_worries
  - utter_goodbye

## survey stop
* greet
  - utter_greet
* affirm
  - health_form
  - form{"name":"health_form"}
* out_of_scope
  - utter_ask_continue
* deny
  - action_deactivate_form
  - form{"name":null}
  - utter_goodbye

## survey continue
* greet
  - utter_greet
* affirm
  - health_form
  - form{"name":"health_form"}
* out_of_scope
  - utter_ask_continue
* affirm
  - health_form
  - form{"name":null}
  - utter_slots_values

## no survey
* greet
  - utter_greet
* deny
  - utter_goodbye

## ask health questions form
* greet
  - utter_greet
* affirm
  - health_form
  - form{"name":"health_form"}
* ask_exercise
  - utter_ask_exercise
  - health_form
  - form{"name":null}
  - utter_goodbye