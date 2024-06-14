export OPENAI_API_KEY=""
export OPENAI_API_BASE=""

python token_benchmark_ray.py \
--model "meta-llama/Meta-Llama-3-70B-Instruct" \
--mean-input-tokens 100 \
--stddev-input-tokens 2 \
--mean-output-tokens 400 \
--stddev-output-tokens 2 \
--max-num-completed-requests 500 \
--timeout 600 \
--num-concurrent-requests 10 \
--results-dir "result_outputs_Llama-3-70B-Instruct_100_400_500_10" \
--llm-api openai \
--additional-sampling-params '{}'
