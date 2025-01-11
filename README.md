# TDS-P1

**>** To scrape data using the GitHub API, first i created a personal access token for authentication, I used python script and parsing the JSON responses to extract the users and repositories data i need.
## Files
1. `users.csv`: Contains information about 475 GitHub users in Zurich with over 50 followers
2. `repositories.csv`: Contains information about 29310 public repositories from these users
3. `tds-p1.ipynb`: Python notebook used to collect this data

##users.csv has following information about each user in Zurich with over 50 followers, with fields:

login: Their Github user ID
name: Their full name
company: The company they work at. Clean up company names. At least make sure:
They're trimmed of whitespace
Leading @ symbol is stripped (Note: ONLY the first one is stripped)
They are converted to UPPERCASE
location: The city they are in
email: Their email address
hireable: Whether they are open to being hired
bio: A short bio about them
public_repos: The number of public repositories they have
followers: The number of followers they have
following: The number of people they are following
created_at: When they joined Github

##repositories.csv has these users' public repositories. For each user in users.csv, fetched up to the 500 most recently pushed repositories, with fields:

login: The Github user ID (login) of the owner, which, BTW, is not directly in the API response.)
full_name: Full name of the repository
created_at: When the repository was created
stargazers_count: Number of stars the repository has
watchers_count: Number of watchers the repository has
language: The programming language the repository is written in
has_projects: Whether the repository has projects enabled
has_wiki: Whether the repository has a wiki
license_name: Name of the license the repository is under (This is under license.key)

**>** One of the most interesting findings from analyzing GitHub data is the strong preference for certain languages among specific user demographics. For instance, while Python and JavaScript dominate overall usage, niche communities showed a surprising affinity for languages like Rust and Go.Users with more contributors and active discussions tend to receive higher stars and forks.

**>** Based on the analysis, an actionable recommendation for developers is to actively engage with their community through regular updates, responsive communication, and encouraging contributions. Establishing a welcoming environment by providing clear contribution guidelines, maintaining an active issue tracker, and fostering discussions can significantly enhance collaboration.

