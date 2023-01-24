# AN INTERMEDIATE REACT FOLDER STRUCTURE

The root of the src fiolder contains index.(js,css) and App.js files. Other folders
are segmented within a signle SRC folder. Helps reduce clatter and the need to search for 
files within multiple folders.

## Pages
Will contain index.js in the root. Each page of the application should then have its own folder 
within the pages folder. Ie Home, About etc. This kind of structure separates page-specific code 
from the more general global code.

## Components
The components folder will have subfolders that keep components separated into different groups
rather than being a big blob of them. For instance, the UI folder can contain user interface 
elements like buttons, cards, modals, etc.

However, for controls that are related to forms like inputs, checkboxes, date pickers etc, they 
are contained in the Form folder. The components folder can be broken down as you see fit but
it should not grow very large as intricate components will be contained in the Pages folder.

## Hooks
The hooks folder stores all the global hooks that are used across various pages. Note that the pages 
folder houses all the page-specific hooks.

## Assets
Images of the project, CSS files, font files etc are stored in this folder

## Context
Context folder stores all the files used on lots of pages. This folder can however be swapped 
with a better folder for storing Redux files if you are using Redux as a global date store.

## Data
Similar to the assets folder, this folder stores data assets such as JSON files. A file containing 
global constant variables may be kept in this directory. These can include enviroemnent variables.

## Utils
The Utils folder stores all the utility features including formatters. the files contained in this
folder need to be simple. You can put pure functions in this directory but there are exceptions to this rule.

*Reference:-->https://dev.to/fpaghar/folder-structuring-techniques-for-beginner-to-advanced-react-projects-30d7*
