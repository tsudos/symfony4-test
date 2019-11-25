# LES COMMANDES  “PHP BIN/CONSOLE”

### Available commands:
<table>
    <thead>
        <tr>
            <th>About //Displays information about the current project</th> 
             <th>help //Displays help for a command</th>  
        </tr>
    </thead>
    <tbody>
        <tr>
            <td> list</td>
            <td>  Lists commands</td>
        </tr>
        <tr>
            <td>
             assets
            </td>
        </tr>
        <tr>
            <td>
                 assets:install
            </td>    
                <td>
                Installs bundles web assets under a public directory
                </td>
        </tr>
        <tr>
            <td>
                cache
            </td>
        </tr>
        <tr>
            <td>
                cache:clear
            </td>    
            <td>
                Clears the cache
            </td>
        </tr>
        <tr>
            <td>
                cache:pool:clear
            </td>    
            <td>
                Clears cache pools
            </td>
        </tr>
        <tr>
            <td>
                cache:pool:delete
                </td>    
                <td>
                Deletes an item from a cache pool
                </td>
        </tr>
        <tr>
            <td>
                cache:pool:prune
            </td>    
            <td>
                Prunes cache pools
            </td>    
        </tr>
        <tr>
            <td>
                cache:warmup
            </td>    
            <td>
                Warms up an empty cache
            </td>
        </td>
        </tr>
        <tr>
            <td>
                doctrine
            </td>
        </tr>
        <tr>
            <td>
                doctrine:cache:clear-collection-region
            </td>    
            <td>
                Clear a second-level cache collection region
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:clear-entity-region
            </td>    
            <td>
                Clear a second-level cache entity region
            </td>          
        </tr>
        <tr>
            <td>
                doctrine:cache:clear-metadata
            </td>    
            <td>
                Clears all metadata cache for an entity manager
            </td>          
          </tr>
        <tr>
            <td>
                doctrine:cache:clear-query 
            </td>    
            <td>
                Clears all query cache for an entity manager
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:clear-query-region
            </td>
            <td>
                Clear a second-level cache query region
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:clear-result
            </td>
            <td>
                Clears result cache for an entity manager
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:contains
            </td>
            <td>    
                Check if a cache entry exists
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:delete
            </td>
            <td>
                Delete a cache entry
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:flush
            </td>
            <td>
                [doctrine:cache:clear] Flush a given cache
            </td>
          </tr>
        <tr>
            <td>
                doctrine:cache:stats
            </td>
            <td>
                Get stats on a given cache provider
            </td>
        </tr>
        <tr>
            <td>
                doctrine:database:create
            </td>
            <td>
                Creates the configured database
            </td>
        </tr>
        <tr>
            <td>
                doctrine:database:drop
            </td>
            <td>
                Drops the configured database
            </td>
        </tr>
        <tr>
            <td>
                doctrine:database:import    
            </td>
            <td>
                Import SQL file(s) directly to Database.
            </td>
        </tr>
        <tr>
            <td>
                 doctrine:ensure-production-settings
            </td>
            <td>
                Verify that Doctrine is properly configured for a production environment
            </td>
        </tr>
        <tr>
            <td>
                doctrine:generate:entities
            </td>
            <td>
                [generate:doctrine:entities] Generates entity classes and methodtubs from your mapping information
            </td>
          </tr>
        <tr>
            <td>
                 doctrine:mapping:convert
            </td>
            <td>
                [orm:convert:mapping] Convert mapping information between suprted formats
            </td>
        </tr>
        <tr>
            <td>
                doctrine:mapping:import
            </td>
            <td>
                Imports mapping information from an existing database
            </td>
        </tr>
        <tr>
            <td>
                doctrine:mapping:info 
            </td>
        </tr>
        <tr>
            <td>
                doctrine:migrations:diff
            </td>
            <td>
                [diff] Generate a migration by comparing your current database tyour mapping information.
            </td>
          </tr>
        <tr>
            <td>
                doctrine:migrations:dump-schema
            </td>
            <td>
                [dump-schema] Dump the schema for your database to a migration.
            </td>
        </tr>
        <tr>
            <td>
                doctrine:migrations:execute
            </td>
            <td> 
                [execute] Execute a single migration version up or down manually.
            </td>
        </tr>
        <tr>
            <td>
                doctrine:migrations:generate
            </td>
            <td>
                [generate] Generate a blank migration class.
         </td>
        </tr>
        <tr>
            <td>
                doctrine:migrations:latest 
            </td>
            <td>
                [latest] Outputs the latest version number
           </td>
          </tr>
        <tr>
            <td>
                doctrine:migrations:migrate
            </td>
            <td>
                [migrate] Execute a migration to a specified version or the latest available version.
           </td>
          </tr>
        <tr>
            <td>
                doctrine:migrations:rollup 
            </td>
            <td>
                [rollup] Rollup migrations by deleting all tracked versions and insert the one version that exists.
           </td>
          </tr>
        <tr>
            <td>
                doctrine:migrations:status
            </td>
            <td>
                [status] View the status of a set of migrations
            </td>        
        </tr>
        <tr>
            <td>
                doctrine:migrations:up-to-date
                
            </td>
            <td>
                [up-to-date] Tells you if your schema is up-to-date.
            </td>    
          </tr>
        <tr>
            <td>
                doctrine:migrations:version
            </td>
            <td>
                [version] Manually add and delete migration versions from the version table.
          </tr>
        <tr>
            <td>
                doctrine:query:dql
            </td>
            <td>
                Executes arbitrary DQL directly from the command line
          </tr>
        <tr>
            <td>
                doctrine:query:sql
            </td>
            <td>
                Executes arbitrary SQL directly from the command line.
          </tr>
        <tr>
            <td>
                doctrine:schema:create 
            </td>
            <td>
                Executes (or dumps) the SQL needed to generate the database schema
          </tr>
        <tr>
            <td>
                doctrine:schema:drop
            </td>
            <td>
                Executes (or dumps) the SQL needed to drop the current database schema
          </tr>
        <tr>
            <td>
                doctrine:schema:update
            </td>
            <td>
                Executes (or dumps) the SQL needed to update the database schema to match the current mapping metadata
          </tr>
        <tr>
            <td>
                doctrine:schema:validate
            </td>
            <td>
                Validate the mapping files
          </tr>
        <tr>
            <td>
                make
            </td>
          </tr>
        <tr>
            <td>
                make:auth
            </td>
            <td>
                Creates a Guard authenticator of different flavors
            </td>
          </tr>
        <tr>
            <td>
                make:command 
            </td>
            <td>
                Creates a new console command class
          </tr>
        <tr>
            <td>
                make:controller
            </td>
            <td>
                Creates a new controller class
          </tr>
        <tr>
            <td>
                make:crud
            </td>
            <td>
                Creates CRUD for Doctrine entity class
          </tr>
        <tr>
            <td>
                make:entity
            </td>
            <td>
                Creates or updates a Doctrine entity class, and optionally an API Platform resource
          </tr>
        <tr>
            <td>
                make:fixtures
            </td>
            <td>
                Creates a new class to load Doctrine fixtures
          </tr>
        <tr>
            <td>
                make:form 
            </td>
            <td>
                Creates a new form class       
        </tr>
        <tr>
            <td>
                make:functional-test 
            </td>
            <td>
                Creates a new functional test class
          </tr>
        <tr>
            <td>
                make:migration
            </td>
            <td>
                Creates a new migration based on database changes
            </td>
          </tr>
        <tr>
            <td>
                make:registration-form 
            </td>
            <td>
                Creates a new registration form system
            </td>
          </tr>
        <tr>
            <td>
                make:serializer:encoder 
            </td>
            <td>
                Creates a new serializer encoder class
            </td>
          </tr>
        <tr>
            <td>
                make:serializer:normalizer 
            </td>
            <td>
                Creates a new serializer normalizer class
            </td>
          </tr>
        <tr>
            <td>
                make:subscriber 
            </td>
            <td>
                Creates a new event subscriber class
            </td>
          </tr>
        <tr>
            <td>
                make:twig-extension 
            </td>
            <td>
                Creates a new Twig extension class
            </td>
          </tr>
        <tr>
            <td>
                make:unit-test
            </td>
            <td>
                Creates a new unit test class
            </td>
          </tr>
        <tr>
            <td>
                make:user 
            </td>
            <td>
                Creates a new security user class
            </td>
          </tr>
        <tr>
            <td>
                make:validator 
            </td>
            <td>
                Creates a new validator and constraint class
            </td>
          </tr>
        <tr>
            <td>
                make:voter
            </td>
            <td>
                Creates a new security voter class
            </td>
            </tr>
        <tr>
            <td>
                server
            <td>
        </tr>
        <tr>
            <td>
                server:dump
            </td>
            <td>
                Starts a dump server that collects and displays dumps in a single place
            </td>
          </tr>
        <tr>
            <td>
                server:log
            </td>
            <td>
                Starts a log server that displays logs in real time
          </tr>
        <tr>
            <td>
                server:run 
            </td>    
            <td>
                Runs a local web server
            </td>
          </tr>
        <tr>
            <td>
                server:start
            </td>    
            <td>
                Starts a local web server in the background
          </tr>
        <tr>
            <td>
                server:status
            </td>    
            <td>    
                Outputs the status of the local web server
            </td>    
          </tr>
        <tr>
            <td>
                server:stop
            </td>    
                <td>
                    Stops the local web server that was started with the server:start 
                </td>
          </tr>
        
