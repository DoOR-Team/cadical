cmake_minimum_required(VERSION 3.13)
project(cadical)

set(CMAKE_CXX_STANDARD 14)

include_directories(src)

add_executable(mobical
        src/analyze.cpp
        src/arena.cpp
        src/arena.hpp
        src/assume.cpp
        src/averages.cpp
        src/averages.hpp
        src/backtrack.cpp
        src/backward.cpp
        src/bins.cpp
        src/bins.hpp
        src/block.cpp
        src/block.hpp
#        src/cadical.cpp
#        src/cadical.hpp
        src/ccadical.cpp
        src/ccadical.h
        src/checker.cpp
        src/checker.hpp
        src/clause.cpp
        src/clause.hpp
        src/collect.cpp
        src/compact.cpp
        src/condition.cpp
        src/config.cpp
        src/config.hpp
        src/contract.cpp
        src/contract.hpp
        src/cover.cpp
        src/cover.hpp
        src/decide.cpp
        src/decompose.cpp
        src/deduplicate.cpp
        src/elim.cpp
        src/elim.hpp
        src/ema.cpp
        src/ema.hpp
        src/extend.cpp
        src/external.cpp
        src/external.hpp
        src/file.cpp
        src/file.hpp
        src/flags.cpp
        src/flags.hpp
        src/format.cpp
        src/format.hpp
        src/gates.cpp
        src/heap.hpp
        src/instantiate.cpp
        src/instantiate.hpp
        src/internal.cpp
        src/internal.hpp
        src/ipasir.cpp
        src/ipasir.h
        src/level.hpp
        src/limit.cpp
        src/limit.hpp
        src/logging.cpp
        src/logging.hpp
        src/lookahead.cpp
        src/lucky.cpp
        src/message.cpp
        src/message.hpp
        src/minimize.cpp
        src/mobical.cpp
        src/observer.hpp
        src/occs.cpp
        src/occs.hpp
        src/options.cpp
        src/options.hpp
        src/parse.cpp
        src/parse.hpp
        src/phases.cpp
        src/phases.hpp
        src/probe.cpp
        src/profile.cpp
        src/profile.hpp
        src/proof.cpp
        src/proof.hpp
        src/propagate.cpp
        src/queue.cpp
        src/queue.hpp
        src/radix.hpp
        src/random.cpp
        src/random.hpp
        src/range.hpp
        src/reduce.cpp
        src/reluctant.hpp
        src/rephase.cpp
        src/report.cpp
        src/resources.cpp
        src/resources.hpp
        src/restart.cpp
        src/restore.cpp
        src/score.cpp
        src/score.hpp
        src/signal.cpp
        src/signal.hpp
        src/solution.cpp
        src/solver.cpp
        src/stats.cpp
        src/stats.hpp
        src/subsume.cpp
        src/terminal.cpp
        src/terminal.hpp
        src/ternary.cpp
        src/tracer.cpp
        src/tracer.hpp
        src/transred.cpp
        src/util.cpp
        src/util.hpp
        src/var.cpp
        src/var.hpp
        src/version.cpp
        src/version.hpp
        src/vivify.cpp
        src/vivify.hpp
        src/walk.cpp
        src/watch.cpp
        src/watch.hpp
#        test/api/apitrace.cpp
#        test/api/cfreeze.c
#        test/api/cipasir.c
#        test/api/ctest.c
#        test/api/example.cpp
#        test/api/learn.cpp
#        test/api/morenmore.cpp
#        test/api/newdelete.cpp
#        test/api/terminate.cpp
#        test/api/traverse.cpp
#        test/api/unit.cpp
#        test/cnf/drat-trim.c
#        test/cnf/precochk.c
        )

add_executable(cadical
        src/analyze.cpp
        src/arena.cpp
        src/arena.hpp
        src/assume.cpp
        src/averages.cpp
        src/averages.hpp
        src/backtrack.cpp
        src/backward.cpp
        src/bins.cpp
        src/bins.hpp
        src/block.cpp
        src/block.hpp
        src/cadical.cpp
        src/cadical.hpp
        src/ccadical.cpp
        src/ccadical.h
        src/checker.cpp
        src/checker.hpp
        src/clause.cpp
        src/clause.hpp
        src/collect.cpp
        src/compact.cpp
        src/condition.cpp
        src/config.cpp
        src/config.hpp
        src/contract.cpp
        src/contract.hpp
        src/cover.cpp
        src/cover.hpp
        src/decide.cpp
        src/decompose.cpp
        src/deduplicate.cpp
        src/elim.cpp
        src/elim.hpp
        src/ema.cpp
        src/ema.hpp
        src/extend.cpp
        src/external.cpp
        src/external.hpp
        src/file.cpp
        src/file.hpp
        src/flags.cpp
        src/flags.hpp
        src/format.cpp
        src/format.hpp
        src/gates.cpp
        src/heap.hpp
        src/instantiate.cpp
        src/instantiate.hpp
        src/internal.cpp
        src/internal.hpp
        src/ipasir.cpp
        src/ipasir.h
        src/level.hpp
        src/limit.cpp
        src/limit.hpp
        src/logging.cpp
        src/logging.hpp
        src/lookahead.cpp
        src/lucky.cpp
        src/message.cpp
        src/message.hpp
        src/minimize.cpp
        #        src/mobical.cpp
        src/observer.hpp
        src/occs.cpp
        src/occs.hpp
        src/options.cpp
        src/options.hpp
        src/parse.cpp
        src/parse.hpp
        src/phases.cpp
        src/phases.hpp
        src/probe.cpp
        src/profile.cpp
        src/profile.hpp
        src/proof.cpp
        src/proof.hpp
        src/propagate.cpp
        src/queue.cpp
        src/queue.hpp
        src/radix.hpp
        src/random.cpp
        src/random.hpp
        src/range.hpp
        src/reduce.cpp
        src/reluctant.hpp
        src/rephase.cpp
        src/report.cpp
        src/resources.cpp
        src/resources.hpp
        src/restart.cpp
        src/restore.cpp
        src/score.cpp
        src/score.hpp
        src/signal.cpp
        src/signal.hpp
        src/solution.cpp
        src/solver.cpp
        src/stats.cpp
        src/stats.hpp
        src/subsume.cpp
        src/terminal.cpp
        src/terminal.hpp
        src/ternary.cpp
        src/tracer.cpp
        src/tracer.hpp
        src/transred.cpp
        src/util.cpp
        src/util.hpp
        src/var.cpp
        src/var.hpp
        src/version.cpp
        src/version.hpp
        src/vivify.cpp
        src/vivify.hpp
        src/walk.cpp
        src/watch.cpp
        src/watch.hpp
        #        test/api/apitrace.cpp
        #        test/api/cfreeze.c
        #        test/api/cipasir.c
        #        test/api/ctest.c
        #        test/api/example.cpp
        #        test/api/learn.cpp
        #        test/api/morenmore.cpp
        #        test/api/newdelete.cpp
        #        test/api/terminate.cpp
        #        test/api/traverse.cpp
        #        test/api/unit.cpp
        #        test/cnf/drat-trim.c
        #        test/cnf/precochk.c
        )

add_library(cadical_lib
        src/analyze.cpp
        src/arena.cpp
        src/arena.hpp
        src/assume.cpp
        src/averages.cpp
        src/averages.hpp
        src/backtrack.cpp
        src/backward.cpp
        src/bins.cpp
        src/bins.hpp
        src/block.cpp
        src/block.hpp
#        src/cadical.cpp
#        src/cadical.hpp
        src/ccadical.cpp
        src/ccadical.h
        src/checker.cpp
        src/checker.hpp
        src/clause.cpp
        src/clause.hpp
        src/collect.cpp
        src/compact.cpp
        src/condition.cpp
        src/config.cpp
        src/config.hpp
        src/contract.cpp
        src/contract.hpp
        src/cover.cpp
        src/cover.hpp
        src/decide.cpp
        src/decompose.cpp
        src/deduplicate.cpp
        src/elim.cpp
        src/elim.hpp
        src/ema.cpp
        src/ema.hpp
        src/extend.cpp
        src/external.cpp
        src/external.hpp
        src/file.cpp
        src/file.hpp
        src/flags.cpp
        src/flags.hpp
        src/format.cpp
        src/format.hpp
        src/gates.cpp
        src/heap.hpp
        src/instantiate.cpp
        src/instantiate.hpp
        src/internal.cpp
        src/internal.hpp
        src/ipasir.cpp
        src/ipasir.h
        src/level.hpp
        src/limit.cpp
        src/limit.hpp
        src/logging.cpp
        src/logging.hpp
        src/lookahead.cpp
        src/lucky.cpp
        src/message.cpp
        src/message.hpp
        src/minimize.cpp
        #        src/mobical.cpp
        src/observer.hpp
        src/occs.cpp
        src/occs.hpp
        src/options.cpp
        src/options.hpp
        src/parse.cpp
        src/parse.hpp
        src/phases.cpp
        src/phases.hpp
        src/probe.cpp
        src/profile.cpp
        src/profile.hpp
        src/proof.cpp
        src/proof.hpp
        src/propagate.cpp
        src/queue.cpp
        src/queue.hpp
        src/radix.hpp
        src/random.cpp
        src/random.hpp
        src/range.hpp
        src/reduce.cpp
        src/reluctant.hpp
        src/rephase.cpp
        src/report.cpp
        src/resources.cpp
        src/resources.hpp
        src/restart.cpp
        src/restore.cpp
        src/score.cpp
        src/score.hpp
        src/signal.cpp
        src/signal.hpp
        src/solution.cpp
        src/solver.cpp
        src/stats.cpp
        src/stats.hpp
        src/subsume.cpp
        src/terminal.cpp
        src/terminal.hpp
        src/ternary.cpp
        src/tracer.cpp
        src/tracer.hpp
        src/transred.cpp
        src/util.cpp
        src/util.hpp
        src/var.cpp
        src/var.hpp
        src/version.cpp
        src/version.hpp
        src/vivify.cpp
        src/vivify.hpp
        src/walk.cpp
        src/watch.cpp
        src/watch.hpp
        )

add_executable(main main.cc)
target_link_libraries(main cadical_lib)