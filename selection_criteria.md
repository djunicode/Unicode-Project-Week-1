# DJ Unicode Project Week

## Selection Criteria

This documents the steps and criteria used for the selection process , which must be adhered to when selecting teams for participation in Unicode project week by the mentors.

### Application process

- Students will need to enter in teams of **3-5 students**, and the application process will be conducted on Devfolio. Participants from all departments are allowed. Students can form teams across departments, but SE and TE students must form separate teams, as final judging will be done separately for SEs and TEs.
- During the initial application - team name, participants’ names and relevant details will be taken as basic information. For selection, following information will also be taken : links to 3 GitHub repositories, at least one problem statement description that they want to work on (maximum 3), and the motivation to enter.
- The GitHub repositories can belong to a single person in a team or can be owned by different people in the team. Repositories of group projects involving people not in the team are allowed, but there should be a considerable amount of commits by the members of the team.
- The scores will be decided by considering all the repositories, not by an individual one. This means a team having 2 good and 1 average repositories will have better scores than a team having 2 average ones and 1 really good.
- The Problem statement entered will be used for team selection, but will not have a score related to it ; detailed explained in the process section below. This PS can be from one of the PS given as general guidelines, a self-created from one of the listed domains, or a self-suggested PS from a domain not listed, but the team wishes to explore. Please see the selection process below to understand how these will be evaluated. Also see the Note related to PS.
- In their motivation to enter, each team should specify what they aim to get out of this : it can be to make a project in a new domain, to explore a new domain or to implement an exciting idea. This will not have any score related to it, but will be used by mentors when selecting the teams.

### Result Process

- After the application phase, the selection process will take place (as explained below). The number of teams selected will depend on the number of mentors, domain selected by team, and a cut off decided for the total marks. As there are a limited number of mentors, a slight preference will be given to uncommon domains and unique (and achievable) problem statements.
- Once the selection is done, the names of selected teams will be announced, and the scores as well as remarks for each team (selected and not-selected) will be made public for all to view. This will ensure transparency during the entire process, and also serve as a guide to non-selected teams for their improvement. That said, the decision made will be final, and can be changed only by internal discussion of Unicode, which may not be made public. This can be done in case of any team found giving false information, or any selected team deciding to withdraw from the event
- In the GitHub repository made by **Unicode** to maintain the documents for this process, a result folder will be created, which will contain a JSON file per team, listing various selection criteria mentioned below, and each having a marks field, and a remarks field, where the marks given and remarks for marks not given will be stated. The remarks field will be used as a suggestion for where the team can improve.
- The JSON format, for example, will be similar to

```json
{
    evaluation:{
        file_structure:{
            score : ‘?/20’,
            remarks : “….”
        },
        naming_convention:{
            score: ‘?/20’,
            remarks: “...”
        }
        …
    }
}
```

- After the result, the selected teams can contact their mentors, and the Project week will take place as per decided timeline.

#### Note Regarding The Problem Statements (PS)

The Unicode Project week aims to focus on _Sustainable_ and _Maintainable_ project development, as well as exploring new domains and topics as a _celebration of learning_. Thus the selection of PS is also guided by this. Unlike other similar events, there is no fixed restrictions on the domains or topics on the PS that a team might choose. There will be some guiding PS given by Unicode as a place to start, or as an idea of possibilities in a domain, from which a team is free to choose or extend a PS. On the other hand, a team is completely free to come up with a PS from the listed domains, or take a PS from a completely different, non-listed domain.

We would be very happy if we could select all teams and help them build a project, but given the finite amount of time and resources, we might not be able to take all teams which apply.

Given that PS is a very nascent idea, and what the selecting mentors understand from the PS given by the team in the application might be different from the idea of the team about the project. Thus, there will be some inevitable selection criteria regarding the PS:

- As we want to encourage exploration of new and unconventional domains, PSs from common and usually selected domains will be given a slightly lower preference.
- A unique or unconventional PS irrespective of domain will be given more preference over common and usually taken topics.
- Combination of above two would result in preference being given to PS from a unique domain, or a really unique PS from a common domain.
- Thus, if you take an unconventional domain from the listed domains, because of the above points, there will be a good chance of a team getting selected, subject to other selection criteria.
- For SEs, even though we really want to encourage exploration of domains which we have not listed, we might not be able to guide the teams posting PS in them. But if a mentor is ready, and wants to explore the domain, your PS might be given higher preference over others.

### Selection Criteria

This section states the criteria to be used for selection of the team, as a guide for both : for the teams to understand how they will be selected, and for mentors to understand how to select the teams. This process will be strictly followed by the mentors during selection of the teams, unless unexpected circumstances occur.

The teams will be judged based on the GitHub repositories of the projects submitted in application, and the PS(s) submitted in application. The marks related to the GitHub repositories are averaged marks after considering all repositories, and not on a single repository. This means two good and one average repositories will be given better marks than two average and one good repositories. The factors to be considered and respective marks are explained in the following points.

1. **Clean coding** : The code files will be checked and the code will be judged for **good coding practices**. For common domains, standard files will be checked : for eg - in Django, views ; in express based projects, models and routes etc. For other domains and non-listed domains code files will be randomly selected and checked based on file names, for eg a file name suggesting core functionality will be checked with more preference than a file name suggesting utility functions ; but this sampling will still be random, and any of the code files can be checked. All of the selected files will be evaluated based on the following points. This section comprise of **20 points**. _Each_ of the individual points below will have 20 points, which will then be averaged to give points for the section.

   - **File structure** : The file structure of the project will be evaluated. If the files are split in appropriate sub folders as required, and overall structure makes sense, it will be given maximum marks allocated.
   - **Naming conventions** of variables, functions, modules etc. : If the variables, functions etc are appropriately named, and help in understanding the code, then for this point complete marks will be given.
   - **Comments** : Comments in the file will be checked according to how much value they add add to the understanding of the code. Unnecessary, or random comments will result in deduction of marks, including commented statements which are usually for debugging purposes (console.log, printf etc). If the comments done (if any) explain the code well, without being an unnecessary bloat, this point will be given complete marks. _Remember, best comments are no comments at all_ - so a good naming convention which requires no comments will also result in complete marks for this point.
   - **Indentation and code formatting** : The code will be checked for consistent and well understandable formatting. A well readable, consistent and understandable formatting will be given complete marks for this point.
   - **Code organization** : The project will be judged for having well separated and sensible code organization. A single file should contain members (functions, classes, variables etc) related to a specific topic or responsibility, and should not be a gigantic monolithic file containing all elements. A well-organized and a well-structured project will be given complete marks for this criterion.
   - **Domain specific conventions** : If the project is from the given list of domains or is in common programming languages or frameworks, it will also be evaluated for domain specific conventions, eg : using arrow functions and async/await in node js etc. This point will be given complete marks if the sampled files follow the domain specific conventions, or if the project is done in some unconventional, esoteric domain, language or framework.
   - **Documentation** : Documentation comments will be judged based on common practices of documenting in respective domains, and is important point of judging for library projects. This might not be considered for application projects. Well written doc comments for exposed API, checked based on sampled files will be given complete marks for this point.

2. **GitHub Commit History** : The project will be judged based on its commit history. This section will have a total of **20 points**. _Each_ of the individual points below will have 20 points, which will then be averaged to give points for the section. A well kept and clean commit history will be given complete marks in this point, which will be evaluated based on following points :

   - **Regular commits** :The commits done should be on a regular or semi-regular intervals, but the commits can vary in interval due to external factors such as college work, or based on bugs found, so irregular commits will still be considered.
   - **Proper commit messages** : All commits should have appropriate and meaningful messages. If most of the commit history adheres to this, this point will be given complete marks.
   - **Sensible commit size** : A single commit should not be too large or contain multiple unrelated changes. Commits will be chosen randomly to check for the amount of changes made and the relevance of the same. If the sampled commits are appropriate in size, and all files changed are relevant to the same issue, this point will be given complete marks. The meaning of relevant is that when adding auth to an app, only files where auth might be relevant should be changed, a change in file related to db, which is not affected by auth, but has some other reason to change will be considered as irrelevant in the same commit.

3. **Readme documentation** : This section comprise of **30 points**. _Each_ of the individual points below will have 30 points, which will then be averaged to give points for the section. Points will be given based on following points, used to evaluate Readme of the project.

   - **Explanation of the project** : Readme should explain what is the project about, why the project was made, why the project is structured the way it is ( as applicable, especially in case of some unique file structuring)
   - **User Documentation** : It should provide documentation in itself, or link to a user documentation regarding the project, explaining how the project is to be used. This is only applicable to application or library based and user related projects. i.e. this is relevant only if the repository contains a project that is supposed to be used as a library or as an application by users, and is not only a proof/exploratory project.
   - **Setup instructions** : Readme MUST provide setup/install and usage instructions. For application projects, this means how to install, setup and run the application, for libraries, this means the API provided by the library, and in other cases this means the setup instructions for the project to be run/setup. If the information is inadequate or not present, it can result in no marks for the Readme, as well as have effect on rest of the sections.
   - **Project Images** : Readme should have images of the running project, maybe along with / inside the user documentation. This point is applicable to application based projects, and might not be considered for library based projects.
   - **Code snippets showing usage** : Readme should have some examples or link to examples of code snippets of the project. This point is only applicable to library based projects, and might not be considered for application projects.
   - **License** : Readme should state information about the project license and optionally the intention behind selection of certain license. The repository should also contain the appropriate license file.
   - Readme should have **only valid and relevant information**, and should not have excessive or irrelevant information. This is more of a soft-criterion, and even though marks may not be deducted for this, it might impact the rest of the points.

4. **Brownie points** : These are extra points that can be awarded by the judging mentors for some unique or extraordinary project submissions. **There is no fixed breakdown of marks** or even points of considerations for this, only restriction is the **maximum points awarded here can be 30**. Note that these marks are completely at the discretion of the judges, and reasons for awarding them may not be explained. However the remark section in results for this might contain information about what points about the project/PS the judges liked/found unique. **Some** points which may be considered for this are, but not limited to :

   - **Hosting the project** : When applicable, hosting or having project in a usable/runnable state may result in points being awarded. Note that appropriate hosting should be considered : For a dynamic application hosting on heroku is reward-able, so is hosting on GitHub pages for static only sites.
   - **Domain, Topic or Framework of Project** : A unique topic of project, an unconventional domain of project or an esoteric stack might result in marks being awarded.

### Selection Process

The selection process will be conducted as follows :

1. First the applications will be collected.
2. A judging team will judge and mark the teams based strictly on above mentioned criteria.
3. The teams will then be sorted according to marks, and based on various factors such as number of teams, range of marks given, a cutoff will be decided.
4. For the teams clearing the cutoff, the mentors of the domains selected will go through the PSs given by the teams, and select the teams for participation. The selection here will depend on :
   - Number of mentors in a specific domain
   - Uniqueness of the PS
   - Judgment of if the PS can actually be done in a week’s time
   - The motivation field
   - The GitHub repositories submitted, etc.
5. These teams will be paired with the mentors that selected them, and the final list of shortlisted teams will be declared.
6. Evaluation of all the teams will be made public, along with their marks and remarks in this repository.
