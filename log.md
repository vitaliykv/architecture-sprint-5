2024-12-11 04:04:19,977 [DEBUG]  Available web server routes: 
/conversations/<conversation_id:path>/messages     POST                           add_message
/conversations/<conversation_id:path>/tracker/events POST                           append_events
/webhooks/rasa                                     GET                            custom_webhook_RasaChatInput.health
/webhooks/rasa/webhook                             POST                           custom_webhook_RasaChatInput.receive
/webhooks/rest                                     GET                            custom_webhook_RestInput.health
/webhooks/rest/webhook                             POST                           custom_webhook_RestInput.receive
/model/test/intents                                POST                           evaluate_intents
/model/test/stories                                POST                           evaluate_stories
/conversations/<conversation_id:path>/execute      POST                           execute_action
/domain                                            GET                            get_domain
/                                                  GET                            hello
/model                                             PUT                            load_model
/model/parse                                       POST                           parse
/conversations/<conversation_id:path>/predict      POST                           predict
/conversations/<conversation_id:path>/tracker/events PUT                            replace_events
/conversations/<conversation_id:path>/story        GET                            retrieve_story
/conversations/<conversation_id:path>/tracker      GET                            retrieve_tracker
/status                                            GET                            status
/model/predict                                     POST                           tracker_predict
/model/train                                       POST                           train
/conversations/<conversation_id:path>/trigger_intent POST                           trigger_intent
/model                                             DELETE                         unload_model
/version                                           GET                            version
2024-12-11 04:04:19,978 [INFO ]  Starting Rasa server on http://0.0.0.0:5005
2024-12-11 04:04:19,979 [DEBUG]  Using the default number of Sanic workers (1).
2024-12-11 04:04:20,084 [DEBUG]  Skipping telemetry reporting: no license hash found.
2024-12-11 04:04:20,111 [DEBUG]  Connected to InMemoryTrackerStore.
2024-12-11 04:04:20,111 [DEBUG]  Connected to lock store 'InMemoryLockStore'.
2024-12-11 04:04:20,112 [DEBUG]  Instantiated NLG to 'TemplatedNaturalLanguageGenerator'.
2024-12-11 04:04:20,112 [INFO ]  Loading model models\20241211-000654-complete-tempo.tar.gz...
2024-12-11 04:04:20,188 [DEBUG]  Extracted model to 'C:\Users\User\AppData\Local\Temp\tmpr0ntf86n'.
2024-12-11 04:04:20,191 [DEBUG]  Node 'nlu_message_converter' loading 'NLUMessageConverter.load' and kwargs: '{}'.
2024-12-11 04:04:20,191 [DEBUG]  Node 'run_WhitespaceTokenizer0' loading 'WhitespaceTokenizer.load' and kwargs: '{}'.
2024-12-11 04:04:20,192 [DEBUG]  Node 'run_RegexFeaturizer1' loading 'RegexFeaturizer.load' and kwargs: '{}'.
2024-12-11 04:04:20,192 [DEBUG]  Resource 'train_RegexFeaturizer1' was requested for reading.
2024-12-11 04:04:20,193 [DEBUG]  Node 'run_LexicalSyntacticFeaturizer2' loading 'LexicalSyntacticFeaturizer.load' and kwargs: '{}'.
2024-12-11 04:04:20,193 [DEBUG]  Resource 'train_LexicalSyntacticFeaturizer2' was requested for reading.
2024-12-11 04:04:20,194 [DEBUG]  Node 'run_CountVectorsFeaturizer3' loading 'CountVectorsFeaturizer.load' and kwargs: '{}'.
2024-12-11 04:04:20,194 [DEBUG]  Resource 'train_CountVectorsFeaturizer3' was requested for reading.
2024-12-11 04:04:20,194 [DEBUG]  Node 'run_LanguageModelFeaturizer4' loading 'LanguageModelFeaturizer.load' and kwargs: '{}'.
2024-12-11 04:04:20,471 [DEBUG]  Loading Tokenizer and Model for bert
2024-12-11 04:04:20,472 [DEBUG]  Starting new HTTPS connection (1): huggingface.co:443
2024-12-11 04:04:20,763 [DEBUG]  https://huggingface.co:443 "HEAD /bert-base-cased/resolve/main/tokenizer_config.json HTTP/1.1" 200 0
2024-12-11 04:04:20,944 [DEBUG]  https://huggingface.co:443 "HEAD /bert-base-cased/resolve/main/config.json HTTP/1.1" 200 0
2024-12-11 04:04:21,699 [DEBUG]  Node 'run_DIETClassifier5' loading 'DIETClassifier.load' and kwargs: '{}'.
2024-12-11 04:04:21,700 [DEBUG]  Resource 'train_DIETClassifier5' was requested for reading.
2024-12-11 04:04:21,700 [DEBUG]  Loading the model from C:\Users\User\AppData\Local\Temp\tmpaunf5jkh\train_DIETClassifier5\DIETClassifier.tf_model with finetune_mode=False...
2024-12-11 04:04:21,709 [DEBUG]  You specified 'DIET' to train entities, but no entities are present in the training data. Skipping training of entities.
2024-12-11 04:04:21,721 [DEBUG]  Following metrics will be logged during training: 
2024-12-11 04:04:21,721 [DEBUG]    t_loss (total loss)
2024-12-11 04:04:21,721 [DEBUG]    i_acc (intent acc)
2024-12-11 04:04:21,721 [DEBUG]    i_loss (intent loss)
2024-12-11 04:04:24,895 [DEBUG]  Finished loading the model.
2024-12-11 04:04:24,895 [DEBUG]  Node 'run_EntitySynonymMapper6' loading 'EntitySynonymMapper.load' and kwargs: '{}'.
2024-12-11 04:04:24,896 [DEBUG]  Resource 'train_EntitySynonymMapper6' was requested for reading.
2024-12-11 04:04:24,896 [DEBUG]  Failed to load ABCMeta from model storage. Resource 'train_EntitySynonymMapper6' doesn't exist.
2024-12-11 04:04:24,896 [DEBUG]  Node 'run_ResponseSelector7' loading 'ResponseSelector.load' and kwargs: '{}'.
2024-12-11 04:04:24,896 [DEBUG]  Resource 'train_ResponseSelector7' was requested for reading.
2024-12-11 04:04:24,897 [DEBUG]  Failed to load ABCMeta from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2024-12-11 04:04:24,897 [DEBUG]  Resource 'train_ResponseSelector7' was requested for reading.
2024-12-11 04:04:24,897 [DEBUG]  Failed to load ResponseSelector from model storage. Resource 'train_ResponseSelector7' doesn't exist.
2024-12-11 04:04:24,897 [DEBUG]  Node 'run_RegexMessageHandler' loading 'RegexMessageHandler.load' and kwargs: '{}'.
2024-12-11 04:04:24,897 [DEBUG]  Node 'domain_provider' loading 'DomainProvider.load' and kwargs: '{}'.
2024-12-11 04:04:24,897 [DEBUG]  Resource 'domain_provider' was requested for reading.
2024-12-11 04:04:24,906 [DEBUG]  Node 'run_MemoizationPolicy0' loading 'MemoizationPolicy.load' and kwargs: '{}'.
2024-12-11 04:04:24,906 [DEBUG]  Resource 'train_MemoizationPolicy0' was requested for reading.
2024-12-11 04:04:24,907 [DEBUG]  Node 'run_RulePolicy1' loading 'RulePolicy.load' and kwargs: '{}'.
2024-12-11 04:04:24,907 [DEBUG]  Resource 'train_RulePolicy1' was requested for reading.
2024-12-11 04:04:24,907 [DEBUG]  Node 'run_UnexpecTEDIntentPolicy2' loading 'UnexpecTEDIntentPolicy.load' and kwargs: '{}'.
2024-12-11 04:04:24,907 [DEBUG]  Resource 'train_UnexpecTEDIntentPolicy2' was requested for reading.
2024-12-11 04:04:24,908 [DEBUG]  Loading the model from C:\Users\User\AppData\Local\Temp\tmpaunf5jkh\train_UnexpecTEDIntentPolicy2\unexpected_intent_policy.tf_model with finetune_mode=False...
2024-12-11 04:04:29,171 [DEBUG]  Finished loading the model.
2024-12-11 04:04:29,171 [WARNI]  The UnexpecTED Intent Policy is currently experimental and might change or be removed in the future 🔬 Please share your feedback on it in the forum (https://forum.rasa.com) to help us make this feature ready for production.
2024-12-11 04:04:29,172 [DEBUG]  Node 'run_TEDPolicy3' loading 'TEDPolicy.load' and kwargs: '{}'.
2024-12-11 04:04:29,172 [DEBUG]  Resource 'train_TEDPolicy3' was requested for reading.
2024-12-11 04:04:29,173 [DEBUG]  Loading the model from C:\Users\User\AppData\Local\Temp\tmpaunf5jkh\train_TEDPolicy3\ted_policy.tf_model with finetune_mode=False...
2024-12-11 04:04:33,041 [DEBUG]  Finished loading the model.
2024-12-11 04:04:33,042 [DEBUG]  Node 'rule_only_data_provider' loading 'RuleOnlyDataProvider.load' and kwargs: '{}'.
2024-12-11 04:04:33,042 [DEBUG]  Resource 'train_RulePolicy1' was requested for reading.
2024-12-11 04:04:33,042 [DEBUG]  Node 'select_prediction' loading 'DefaultPolicyPredictionEnsemble.load' and kwargs: '{}'.
2024-12-11 04:04:33,046 [INFO ]  Rasa server is up and running.
2024-12-11 04:04:33,047 [INFO ]  Enabling coroutine debugging. Loop id 2949519801648.
2024-12-11 04:04:49,936 [DEBUG]  Issuing ticket for conversation 'PractikumStudent'.
2024-12-11 04:04:49,936 [DEBUG]  Acquiring lock for conversation 'PractikumStudent'.
2024-12-11 04:04:49,936 [DEBUG]  Acquired lock for conversation 'PractikumStudent'.
2024-12-11 04:04:49,936 [DEBUG]  Could not find tracker for conversation ID 'PractikumStudent'.
2024-12-11 04:04:49,936 [DEBUG]  No event broker configured. Skipping streaming events.
2024-12-11 04:04:49,937 [DEBUG]  Starting a new session for conversation ID 'PractikumStudent'.
2024-12-11 04:04:49,938 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.policy_prediction[0m [36mprediction_events[0m=[35m[][0m
2024-12-11 04:04:49,938 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.log         [0m [36maction_name[0m=[35maction_session_start[0m [36mrasa_events[0m=[35m[<rasa.shared.core.events.SessionStarted object at 0x000002AF09DF8760>, ActionExecuted(action: action_listen, policy: None, confidence: None)][0m
2024-12-11 04:04:49,938 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.slots.log           [0m [36mslot_values[0m=[35m	topic: None
	session_started_metadata: None[0m
2024-12-11 04:04:49,939 [DEBUG]  Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x000002AF09DF10A0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1460>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:04:49,939 [DEBUG]  Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2024-12-11 04:04:49,939 [DEBUG]  Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2024-12-11 04:04:49,939 [DEBUG]  Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2024-12-11 04:04:49,940 [DEBUG]  Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2024-12-11 04:04:49,940 [DEBUG]  Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2024-12-11 04:04:49,940 [DEBUG]  Node 'run_LanguageModelFeaturizer4' running 'LanguageModelFeaturizer.process'.
2024-12-11 04:04:50,146 [DEBUG]  Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2024-12-11 04:04:50,214 [DEBUG]  Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2024-12-11 04:04:50,214 [DEBUG]  Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2024-12-11 04:04:50,214 [DEBUG]  There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2024-12-11 04:04:50,214 [DEBUG]  Adding following selector key to message property: default
2024-12-11 04:04:50,215 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:04:50,215 [DEBUG]  Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2024-12-11 04:04:50,216 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.message.parse       [0m [36mparse_data_entities[0m=[35m[][0m [36mparse_data_intent[0m=[35m{'name': 'greet', 'confidence': 0.40638267993927}[0m [36mparse_data_text[0m=[35mКакие подходы существуют в архитектуре?[0m
2024-12-11 04:04:50,216 [DEBUG]  Logged UserUtterance - tracker now has 4 events.
2024-12-11 04:04:50,217 [DEBUG]  Validating extracted slots: topic
2024-12-11 04:04:50,217 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.extract.slots       [0m [36maction_extract_slot[0m=[35maction_extract_slots[0m [36mlen_extraction_events[0m=[35m1[0m [36mrasa_events[0m=[35m[SlotSet(key: topic, value: Какие подходы существуют в архитектуре?)][0m
2024-12-11 04:04:50,217 [DEBUG]  Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1460>}, targets: ['select_prediction'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:04:50,217 [DEBUG]  Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2024-12-11 04:04:50,218 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:04:50,218 [DEBUG]  Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,218 [DEBUG]  [[32m[1mdebug    [0m] [1mmemoization.predict.actions   [0m [36mtracker_states[0m=[35m[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}][0m
2024-12-11 04:04:50,218 [DEBUG]  There is a memorised next action 'utter_greet'
2024-12-11 04:04:50,218 [DEBUG]  Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2024-12-11 04:04:50,218 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user text: Какие подходы существуют в архитектуре? | previous action name: action_listen[0m
2024-12-11 04:04:50,219 [DEBUG]  There is no applicable rule.
2024-12-11 04:04:50,219 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user intent: greet | previous action name: action_listen[0m
2024-12-11 04:04:50,219 [DEBUG]  There is a rule for the next action 'utter_greet'.
2024-12-11 04:04:50,219 [DEBUG]  Node 'run_TEDPolicy3' running 'TEDPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,221 [DEBUG]  TED predicted 'utter_greet' based on user intent.
2024-12-11 04:04:50,221 [DEBUG]  Node 'run_UnexpecTEDIntentPolicy2' running 'UnexpecTEDIntentPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,349 [DEBUG]  Querying for intent `greet`.
2024-12-11 04:04:50,349 [DEBUG]  Score for intent `greet` is `1.4680278301239014`, while threshold is `-1.685218095779419`.
2024-12-11 04:04:50,349 [DEBUG]  Top 5 intents (in ascending order) that are likely here are: `[('affirm', -1.802249), ('ask_architecture', -1.479586), ('request_info', 0.63579404), ('goodbye', 1.0783516), ('greet', 1.4680278)]`.
2024-12-11 04:04:50,349 [DEBUG]  Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2024-12-11 04:04:50,350 [DEBUG]  Made prediction using user intent.
2024-12-11 04:04:50,350 [DEBUG]  Added `DefinePrevUserUtteredFeaturization(False)` event.
2024-12-11 04:04:50,350 [DEBUG]  Predicted next action using RulePolicy.
2024-12-11 04:04:50,350 [DEBUG]  Predicted next action 'utter_greet' with confidence 1.00.
2024-12-11 04:04:50,351 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.policy_prediction[0m [36mprediction_events[0m=[35m[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x000002AF09DF1070>][0m
2024-12-11 04:04:50,351 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.log         [0m [36maction_name[0m=[35mutter_greet[0m [36mrasa_events[0m=[35m[BotUttered('Привет! Чем могу помочь в области архитектуры программного обеспечения?', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_greet"}, 1733879090.3503094)][0m
2024-12-11 04:04:50,351 [DEBUG]  Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1460>}, targets: ['select_prediction'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:04:50,351 [DEBUG]  Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2024-12-11 04:04:50,351 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:04:50,351 [DEBUG]  Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,352 [DEBUG]  [[32m[1mdebug    [0m] [1mmemoization.predict.actions   [0m [36mtracker_states[0m=[35m[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}][0m
2024-12-11 04:04:50,352 [DEBUG]  There is a memorised next action 'action_listen'
2024-12-11 04:04:50,352 [DEBUG]  Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2024-12-11 04:04:50,352 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet[0m
2024-12-11 04:04:50,352 [DEBUG]  There is a rule for the next action 'action_listen'.
2024-12-11 04:04:50,352 [DEBUG]  Node 'run_TEDPolicy3' running 'TEDPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,354 [DEBUG]  TED predicted 'action_listen' based on user intent.
2024-12-11 04:04:50,354 [DEBUG]  Node 'run_UnexpecTEDIntentPolicy2' running 'UnexpecTEDIntentPolicy.predict_action_probabilities'.
2024-12-11 04:04:50,354 [DEBUG]  Skipping predictions for UnexpecTEDIntentPolicy as either there is no event of type `UserUttered`, event's intent is new and not in domain or there is an event of type `ActionExecuted` after the last `UserUttered`.
2024-12-11 04:04:50,354 [DEBUG]  Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2024-12-11 04:04:50,354 [DEBUG]  Predicted next action using RulePolicy.
2024-12-11 04:04:50,355 [DEBUG]  Predicted next action 'action_listen' with confidence 1.00.
2024-12-11 04:04:50,355 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.policy_prediction[0m [36mprediction_events[0m=[35m[][0m
2024-12-11 04:04:50,355 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.log         [0m [36maction_name[0m=[35maction_listen[0m [36mrasa_events[0m=[35m[][0m
2024-12-11 04:04:50,355 [DEBUG]  No event broker configured. Skipping streaming events.
2024-12-11 04:04:50,355 [DEBUG]  Deleted lock for conversation 'PractikumStudent'.
2024-12-11 04:06:44,640 [DEBUG]  Issuing ticket for conversation 'PractikumStudent'.
2024-12-11 04:06:44,640 [DEBUG]  Acquiring lock for conversation 'PractikumStudent'.
2024-12-11 04:06:44,640 [DEBUG]  Acquired lock for conversation 'PractikumStudent'.
2024-12-11 04:06:44,640 [DEBUG]  Recreating tracker for id 'PractikumStudent'
2024-12-11 04:06:44,641 [DEBUG]  Running graph with inputs: {'__message__': [<rasa.core.channels.channel.UserMessage object at 0x000002AF09DF84F0>], '__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1C70>}, targets: ['run_RegexMessageHandler'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:06:44,642 [DEBUG]  Node 'nlu_message_converter' running 'NLUMessageConverter.convert_user_message'.
2024-12-11 04:06:44,643 [DEBUG]  Node 'run_WhitespaceTokenizer0' running 'WhitespaceTokenizer.process'.
2024-12-11 04:06:44,643 [DEBUG]  Node 'run_RegexFeaturizer1' running 'RegexFeaturizer.process'.
2024-12-11 04:06:44,643 [DEBUG]  Node 'run_LexicalSyntacticFeaturizer2' running 'LexicalSyntacticFeaturizer.process'.
2024-12-11 04:06:44,643 [DEBUG]  Node 'run_CountVectorsFeaturizer3' running 'CountVectorsFeaturizer.process'.
2024-12-11 04:06:44,644 [DEBUG]  Node 'run_LanguageModelFeaturizer4' running 'LanguageModelFeaturizer.process'.
2024-12-11 04:06:44,750 [DEBUG]  Node 'run_DIETClassifier5' running 'DIETClassifier.process'.
2024-12-11 04:06:44,752 [DEBUG]  Node 'run_EntitySynonymMapper6' running 'EntitySynonymMapper.process'.
2024-12-11 04:06:44,752 [DEBUG]  Node 'run_ResponseSelector7' running 'ResponseSelector.process'.
2024-12-11 04:06:44,752 [DEBUG]  There is no trained model for 'ResponseSelector': The component is either not trained or didn't receive enough training data.
2024-12-11 04:06:44,752 [DEBUG]  Adding following selector key to message property: default
2024-12-11 04:06:44,753 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:06:44,753 [DEBUG]  Node 'run_RegexMessageHandler' running 'RegexMessageHandler.process'.
2024-12-11 04:06:44,753 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.message.parse       [0m [36mparse_data_entities[0m=[35m[][0m [36mparse_data_intent[0m=[35m{'name': 'goodbye', 'confidence': 0.4608663320541382}[0m [36mparse_data_text[0m=[35mПривет[0m
2024-12-11 04:06:44,753 [DEBUG]  Logged UserUtterance - tracker now has 10 events.
2024-12-11 04:06:44,753 [DEBUG]  Validating extracted slots: topic
2024-12-11 04:06:44,753 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.extract.slots       [0m [36maction_extract_slot[0m=[35maction_extract_slots[0m [36mlen_extraction_events[0m=[35m1[0m [36mrasa_events[0m=[35m[SlotSet(key: topic, value: Привет)][0m
2024-12-11 04:06:44,754 [DEBUG]  Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1C70>}, targets: ['select_prediction'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:06:44,754 [DEBUG]  Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2024-12-11 04:06:44,754 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:06:44,754 [DEBUG]  Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,754 [DEBUG]  [[32m[1mdebug    [0m] [1mmemoization.predict.actions   [0m [36mtracker_states[0m=[35m[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'goodbye'}, 'prev_action': {'action_name': 'action_listen'}}][0m
2024-12-11 04:06:44,754 [DEBUG]  There is no memorised next action
2024-12-11 04:06:44,754 [DEBUG]  Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2024-12-11 04:06:44,755 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user text: Привет | previous action name: action_listen[0m
2024-12-11 04:06:44,755 [DEBUG]  There is no applicable rule.
2024-12-11 04:06:44,755 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: goodbye | previous action name: action_listen[0m
2024-12-11 04:06:44,755 [DEBUG]  There is a rule for the next action 'utter_goodbye'.
2024-12-11 04:06:44,755 [DEBUG]  Node 'run_TEDPolicy3' running 'TEDPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,758 [DEBUG]  TED predicted 'utter_goodbye' based on user intent.
2024-12-11 04:06:44,758 [DEBUG]  Node 'run_UnexpecTEDIntentPolicy2' running 'UnexpecTEDIntentPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,759 [DEBUG]  Querying for intent `goodbye`.
2024-12-11 04:06:44,760 [DEBUG]  Score for intent `goodbye` is `-1.5643599033355713`, while threshold is `-1.5643599033355713`.
2024-12-11 04:06:44,760 [DEBUG]  Top 5 intents (in ascending order) that are likely here are: `[('request_info', -1.5861583), ('goodbye', -1.5643599), ('nlu_fallback', -1.5422654), ('session_start', -1.5213504), ('ask_architecture', 1.6462876)]`.
2024-12-11 04:06:44,760 [DEBUG]  Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2024-12-11 04:06:44,760 [DEBUG]  Made prediction using user intent.
2024-12-11 04:06:44,760 [DEBUG]  Added `DefinePrevUserUtteredFeaturization(False)` event.
2024-12-11 04:06:44,760 [DEBUG]  Predicted next action using RulePolicy.
2024-12-11 04:06:44,760 [DEBUG]  Predicted next action 'utter_goodbye' with confidence 1.00.
2024-12-11 04:06:44,760 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.policy_prediction[0m [36mprediction_events[0m=[35m[<rasa.shared.core.events.DefinePrevUserUtteredFeaturization object at 0x000002AEBF1ABB50>][0m
2024-12-11 04:06:44,761 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.log         [0m [36maction_name[0m=[35mutter_goodbye[0m [36mrasa_events[0m=[35m[BotUttered('До свидания! Если появятся вопросы по архитектуре ПО, обращайтесь.', {"elements": null, "quick_replies": null, "buttons": null, "attachment": null, "image": null, "custom": null}, {"utter_action": "utter_goodbye"}, 1733879204.7605796)][0m
2024-12-11 04:06:44,761 [DEBUG]  Running graph with inputs: {'__tracker__': <rasa.shared.core.trackers.DialogueStateTracker object at 0x000002AF09DF1C70>}, targets: ['select_prediction'] and ExecutionContext(model_id='6d029f3c1f8e4a458d572c44c86e67b9', should_add_diagnostic_data=False, is_finetuning=False, node_name=None).
2024-12-11 04:06:44,761 [DEBUG]  Node 'rule_only_data_provider' running 'RuleOnlyDataProvider.provide'.
2024-12-11 04:06:44,761 [DEBUG]  Node 'domain_provider' running 'DomainProvider.provide_inference'.
2024-12-11 04:06:44,761 [DEBUG]  Node 'run_MemoizationPolicy0' running 'MemoizationPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,761 [DEBUG]  [[32m[1mdebug    [0m] [1mmemoization.predict.actions   [0m [36mtracker_states[0m=[35m[{}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'greet'}, 'prev_action': {'action_name': 'utter_greet'}}, {'user': {'intent': 'goodbye'}, 'prev_action': {'action_name': 'action_listen'}}, {'user': {'intent': 'goodbye'}, 'prev_action': {'action_name': 'utter_goodbye'}}][0m
2024-12-11 04:06:44,761 [DEBUG]  There is no memorised next action
2024-12-11 04:06:44,761 [DEBUG]  Node 'run_RulePolicy1' running 'RulePolicy.predict_action_probabilities'.
2024-12-11 04:06:44,762 [DEBUG]  [[32m[1mdebug    [0m] [1mrule_policy.actions.find      [0m [36mcurrent_states[0m=[35m
[state 1] user intent: greet | previous action name: action_listen
[state 2] user intent: greet | previous action name: utter_greet
[state 3] user intent: goodbye | previous action name: action_listen
[state 4] user intent: goodbye | previous action name: utter_goodbye[0m
2024-12-11 04:06:44,762 [DEBUG]  There is a rule for the next action 'action_listen'.
2024-12-11 04:06:44,762 [DEBUG]  Node 'run_TEDPolicy3' running 'TEDPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,764 [DEBUG]  TED predicted 'action_listen' based on user intent.
2024-12-11 04:06:44,764 [DEBUG]  Node 'run_UnexpecTEDIntentPolicy2' running 'UnexpecTEDIntentPolicy.predict_action_probabilities'.
2024-12-11 04:06:44,764 [DEBUG]  Skipping predictions for UnexpecTEDIntentPolicy as either there is no event of type `UserUttered`, event's intent is new and not in domain or there is an event of type `ActionExecuted` after the last `UserUttered`.
2024-12-11 04:06:44,764 [DEBUG]  Node 'select_prediction' running 'DefaultPolicyPredictionEnsemble.combine_predictions_from_kwargs'.
2024-12-11 04:06:44,764 [DEBUG]  Predicted next action using RulePolicy.
2024-12-11 04:06:44,764 [DEBUG]  Predicted next action 'action_listen' with confidence 1.00.
2024-12-11 04:06:44,764 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.policy_prediction[0m [36mprediction_events[0m=[35m[][0m
2024-12-11 04:06:44,764 [DEBUG]  [[32m[1mdebug    [0m] [1mprocessor.actions.log         [0m [36maction_name[0m=[35maction_listen[0m [36mrasa_events[0m=[35m[][0m
2024-12-11 04:06:44,764 [DEBUG]  No event broker configured. Skipping streaming events.
2024-12-11 04:06:44,764 [DEBUG]  Deleted lock for conversation 'PractikumStudent'.
