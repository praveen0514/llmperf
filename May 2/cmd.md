export OPENAI_API_KEY="" export OPENAI_API_BASE=""

python token_benchmark_ray.py \
--model "llama-3-70b-instruct" \
--mean-input-tokens 400 \
--stddev-input-tokens 2 \
--mean-output-tokens 100 \
--stddev-output-tokens 2 \
--max-num-completed-requests 500 \
--timeout 600 \
--num-concurrent-requests 10 \
--results-dir "result_outputs_May2_llama-3-70b-instruct_400_100_500_10" \
--llm-api openai \
--additional-sampling-params '{}'
