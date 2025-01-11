# TDS-P1

**>** To scrape data using the GitHub API, first i created a personal access token for authentication, I used python script and parsing the JSON responses to extract the users and repositories data i need.
## Files
1. `users.csv`: Contains information about 475 GitHub users in Zurich with over 50 followers
2. `repositories.csv`: Contains information about 29310 public repositories from these users
3. `tds-p1.ipynb`: Python notebook used to collect this data

## users.csv has following information about each user in Zurich with over 50 followers, with fields:

1. login: Their Github user ID
2. name: Their full name
3. company: The company they work at.
4. location: The city they are in
5. email: Their email address
6. hireable: Whether they are open to being hired
7. bio: A short bio about them
8. public_repos: The number of public repositories they have
9. followers: The number of followers they have
10. following: The number of people they are following
11. created_at: When they joined Github

## repositories.csv has these users' public repositories. For each user in users.csv, fetched up to the 500 most recently pushed repositories, with fields:

1. login: The Github user ID (login) of the owner, which, BTW, is not directly in the API response.
2. full_name: Full name of the repository
3. created_at: When the repository was created
4. stargazers_count: Number of stars the repository has
5. watchers_count: Number of watchers the repository has
6. language: The programming language the repository is written in
7. has_projects: Whether the repository has projects enabled
8. has_wiki: Whether the repository has a wiki
9. license_name: Name of the license the repository is under (This is under license.key)

## OBSERVATIONS

**>** One of the most interesting findings from analyzing GitHub data is the strong preference for certain languages among specific user demographics. For instance, while Python and JavaScript dominate overall usage, niche communities showed a surprising affinity for languages like Rust and Go.Users with more contributors and active discussions tend to receive higher stars and forks.

**>** Based on the analysis, an actionable recommendation for developers is to actively engage with their community through regular updates, responsive communication, and encouraging contributions. Establishing a welcoming environment by providing clear contribution guidelines, maintaining an active issue tracker, and fostering discussions can significantly enhance collaboration.

