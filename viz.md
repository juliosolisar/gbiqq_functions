```r
library(pkgnet)
report1 <- CreatePackageReport(pkg_name = "gbiqq")


#all_data_types
#gives a table of all possible data types given the model
variables <- model$variables 
m <- length(model$variables)
df <- data.frame(perm(rep(2, m))) - 1
df[df == -1] <- NA
names(df) <- variables
data.frame(cbind(event = data_type_names(model, df), df))

any_discrepancies	Check for discrepancies Used in make_alphas
check_params	Check parameters sum to 1 in paramset and normalize

clean_condition	Clean condition
collapse_data	Make data compact with data as first argument
combine_lists	combine two lists by names
data_strategy	Data Strategy
data_type_names	Data type names
democracy_data	Democracy Data
draw_data_events	Draw compact data
draw_event_prob	Draw event probabilities
draw_parameters	Draw parameters Default behavior takes a random draw of parameters from priors; can also draw from posteriors, or return pre-defined parameters.
draw_type_prob	Draw type probabilities
draw_type_prob_multiple	Draw matrix of type probabilities, before or after estimation
encode_data	Encode data
expand_wildcard	Expand wildcard
fitted_model	Generate a fitted stan model
gbiqq	Fit stan model
get_ambiguities_matrix	Get ambiguities matrix
get_causal_types	Get causal types
get_data_events	Summarize data events
get_likelihood_helpers	get_likelihood_helpers
get_max_possible_data	Get data frame with all possible data combinations
get_nodal_types	Get list of types for variables in a DAG
get_parameters	Get parameters
get_parameter_matrix	Get parameter matrix
get_parameter_names	get_parameter_names
get_param_set_names	Get names of groups in param_set
get_parents	Get list of parents in a dag
get_possible_data	Get Possible Data
get_priors	Get prior distribution
get_types	Get values of types according to a query
get_type_names	Get type names
gsub_many	Recursive substitution
includes_var	Whether a query contains an exact string
interpret_type	Interpret or find position in nodal type
lookup_type	Lookup nodal types according to a query
lookup_type_internal	Reveal nodal types according to a query
make_alphas	Make alphas
make_ambiguities_matrix	Make ambiguities matrix
make_gbiqq_data	Prepare data for stan
make_model	Make a model
make_parameter_matrix	Make parameter matrix
make_priors	Make priors
observe	Observe data, given a strategy
perm	Produces the possible permutations of a set of variables
plot_dag	Plot your dag using dagitty
query_distribution	Calculate estimand distribution
query_model	Generate estimands dataframe
reduce_parameters	Reduce parameters If parameters is longer than nodel types, because of a model restriction, subset lambda and renormalize
restrict_nodal_types_exp	Reduce nodal types
restrict_nodal_types_labels	Reduce nodal types
reveal_outcomes	Reveal outcomes
set_ambiguities_matrix	Set ambiguity matrix
set_confound	Set confound
set_parameters	Add a true parameter vector
set_parameter_matrix	Set parameter matrix
set_priors	Set prior distribution
set_prior_distribution	Add prior distribution draws
set_restrictions	Restrict a model
simulate_data	Generate full dataset, possibly from compact data
st_within	Get string between two regular expression patterns
summarize_data	Summarize Data
translate_dagitty	Puts your DAG into daggity syntax (useful for using their plotting functions)
types_to_nodes	Wrapper of types_to_nodes_single Sapply multiple query conditions
type_matrix	Generate type matrix
unpack_wildcard	Unpack a wild card
update_causal_types	Update causal types based on nodal types
var_in_query	List of variables contained in query
```

