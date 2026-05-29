# Fine-Tuning a "Doosmday" GPT

*After a devastating decapitation strike on the U.S. government in 2034, a military coup seized power and launched a pre-emptive nuclear exchange, fundamentally altering the global energy and geopolitical landscape. Today, the nation survives isolated behind a high-tech missile defense shield, its people united under the myth that Divine Providence saved America from global destruction.*

This is the state of the world that the GPT model I fine-tuned exists in. With the help of Gemini and Claude, the Jupyter Notebook in this repository includes a fine-tuned LLM based on the world I created. A variety of different pieces of information were created, also using Gemini, to train this model. In order to give the model personality and a grounding in the world created, prompt/answer pairs were used for training and along with mock pieces of legislation, radio tranmissions, newspapers, and historical documents.  

Here is the local evaluation of test prompts: 

Both `max_new_tokens` (=120) and `max_length`(=131072) seem to have been set. `max_new_tokens` will take precedence. Please refer to the documentation for more information. (https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)

🔍 Running evaluation suite…

Both `max_new_tokens` (=120) and `max_length`(=131072) seem to have been set. `max_new_tokens` will take precedence. Please refer to the documentation for more information. (https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)
───────────────────────────────────────────────────────
  Instruction : Query status of the Atlantic Wall and report any foreign signals.
  Response    : The Atlantic Wall remains a solid barrier of high-tension steel, effectively sealing our nation against the entropic fir…
───────────────────────────────────────────────────────
  Persona keywords  : 2.0 / 4
  Fluency (ppl)     : 4.0 / 4
  Repetition ratio  : 2.0 / 2
  TOTAL SCORE       : 8.0 / 10

/usr/local/lib/python3.12/dist-packages/transformers/modeling_attn_mask_utils.py:71: FutureWarning: The attention mask API under `transformers.modeling_attn_mask_utils` (`AttentionMaskConverter`) is deprecated and will be removed in Transformers v5.10. Please use the new API in `transformers.masking_utils`.
  warnings.warn(DEPRECATION_MESSAGE, FutureWarning)
/usr/local/lib/python3.12/dist-packages/transformers/modeling_attn_mask_utils.py:281: FutureWarning: The attention mask API under `transformers.modeling_attn_mask_utils` (`AttentionMaskConverter`) is deprecated and will be removed in Transformers v5.10. Please use the new API in `transformers.masking_utils`.
  warnings.warn(DEPRECATION_MESSAGE, FutureWarning)
Both `max_new_tokens` (=120) and `max_length`(=131072) seem to have been set. `max_new_tokens` will take precedence. Please refer to the documentation for more information. (https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)
───────────────────────────────────────────────────────
  Instruction : What does a sentinel do?
  Response    : A Sentinel's primary function is to monitor the exterior perimeter of the Habitation Block using thermal-imaging and aco…
───────────────────────────────────────────────────────
  Persona keywords  : 2.0 / 4
  Fluency (ppl)     : 4.0 / 4
  Repetition ratio  : 2.0 / 2
  TOTAL SCORE       : 8.0 / 10

Both `max_new_tokens` (=120) and `max_length`(=131072) seem to have been set. `max_new_tokens` will take precedence. Please refer to the documentation for more information. (https://huggingface.co/docs/transformers/main/en/main_classes/text_generation)
───────────────────────────────────────────────────────
  Instruction : Describe the Richmond Mandate.
  Response    : The mandate establishes the 'Totality of Trust' between the Protector and his workforce, ensuring that all labor is perf…
───────────────────────────────────────────────────────
  Persona keywords  : 4.0 / 4
  Fluency (ppl)     : 4.0 / 4
  Repetition ratio  : 2.0 / 2
  TOTAL SCORE       : 10.0 / 10

───────────────────────────────────────────────────────
  Instruction : Report anomalous transmissions detected in Sector 7.
  Response    : Spectral analysis confirms that these signals are originating from an ancient high-frequency shortwave band used by pre-…
───────────────────────────────────────────────────────
  Persona keywords  : 2.0 / 4
  Fluency (ppl)     : 4.0 / 4
  Repetition ratio  : 2.0 / 2
  TOTAL SCORE       : 8.0 / 10

=======================================================
SUMMARY
=======================================================
   8.0/10  ████████    Query status of the Atlantic Wall and report 
   8.0/10  ████████    What does a sentinel do?
  10.0/10  ██████████  Describe the Richmond Mandate.
   8.0/10  ████████    Report anomalous transmissions detected in Se

  Average score: 8.5 / 10
